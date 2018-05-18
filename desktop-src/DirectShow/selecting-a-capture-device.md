---
Description: Selecting a Capture Device
ms.assetid: '8f92873d-569a-48af-a913-6d4cce65640f'
title: Selecting a Capture Device
---

# Selecting a Capture Device

To select an audio or video capture device, use the [System Device Enumerator](system-device-enumerator.md), described in the topic [Using the System Device Enumerator](using-the-system-device-enumerator.md). The System Device Enumerator returns a collection of device monikers, selected by device category. A *moniker* is a COM object that contains information about another object. Monikers enable the application to get information about an object without actually creating the object. Later, the application can use the moniker to create the object. For more information about monikers, see the documentation for [**IMoniker**](com.imoniker).

To use the System Device Enumerator, perform the following steps.

1.  Call [**CoCreateInstance**](com.cocreateinstance) to create an instance of the System Device Enumerator.
2.  Call [**ICreateDevEnum::CreateClassEnumerator**](icreatedevenum-createclassenumerator.md) and specify the device category as a GUID. For capture devices, the following categories are relevant. 

    | Category GUID                       | Description           |
    |-------------------------------------|-----------------------|
    | **CLSID\_AudioInputDeviceCategory** | Audio capture devices |
    | **CLSID\_VideoInputDeviceCategory** | Video capture devices |

    

     

    If a video camera has an integrated microphone, it appears in both categories. However, the camera and microphone are treated as separate devices by the system, for purposes of enumeration, device creation, and data streaming.

3.  The [**CreateClassEnumerator**](icreatedevenum-createclassenumerator.md) method returns a pointer to the [**IEnumMoniker**](com.ienummoniker) interface. To enumerate the monikers, call [**IEnumMoniker::Next**](com.ienummoniker_next).

The following code creates an enumerator for a specified device category.


```C++
#include <windows.h>
#include <dshow.h>

#pragma comment(lib, "strmiids")

HRESULT EnumerateDevices(REFGUID category, IEnumMoniker **ppEnum)
{
    // Create the System Device Enumerator.
    ICreateDevEnum *pDevEnum;
    HRESULT hr = CoCreateInstance(CLSID_SystemDeviceEnum, NULL,  
        CLSCTX_INPROC_SERVER, IID_PPV_ARGS(&amp;pDevEnum));

    if (SUCCEEDED(hr))
    {
        // Create an enumerator for the category.
        hr = pDevEnum->CreateClassEnumerator(category, ppEnum, 0);
        if (hr == S_FALSE)
        {
            hr = VFW_E_NOT_FOUND;  // The category is empty. Treat as an error.
        }
        pDevEnum->Release();
    }
    return hr;
}
```



The [**IEnumMoniker**](com.ienummoniker) interface enumerates a list of [**IMoniker**](com.imoniker) interfaces, each of which represents a device moniker. The application can read properties from the moniker, or use the moniker to create a DirectShow capture filter for the device. Moniker properties are returned as **VARIANT** values. The following properties are supported by device monikers.



| Property       | Description                                                               | VARIANT Type |
|----------------|---------------------------------------------------------------------------|--------------|
| "FriendlyName" | The name of the device.                                                   | **VT\_BSTR** |
| "Description"  | A description of the device.                                              | **VT\_BSTR** |
| "DevicePath"   | A unique string that identifies the device. (Video capture devices only.) | **VT\_BSTR** |
| "WaveInID"     | The identifier for an audio capture device. (Audio capture devices only.) | **VT\_I4**   |



 

The "FriendlyName" and "Description" properties are suitable for displaying in a UI.

-   The "FriendlyName" property is available for every device. It contains a human-readable name for the device.
-   The "Description" property is available only for DV and D-VHS/MPEG camcorder devices. For more information, see [MSDV Driver](msdv-driver.md) and [MSTape Driver](mstape-driver.md). If available, it contains a description of the device which is more specific than the "FriendlyName" property. Typically it includes the vendor name.
-   The "DevicePath" property is not a human-readable string, but is guaranteed to be unique for each video capture device on the system. You can use this property to distinguish between two or more instances of the same model of device.
-   If the "WaveInID" property is present, it means the DirectShow capture filter uses the [Waveform Audio](multimedia.waveform_audio) APIs internally to communicate with the device. The value of the "WaveInID" property corresponds to the identifier used by the **waveIn\*** functions, such as [**waveInOpen**](multimedia.waveinopen).

To read properties from the moniker, perform the following steps.

1.  Call [**IMoniker::BindToStorage**](com.imoniker_bindtostorage) to get a pointer to the [**IPropertyBag**](com.ipropertybag_and_ipersistpropertybag) interface.
2.  Call **IPropertyBag::Read** to read the property.

The following code example shows how to enumerate a list of device monikers and get the properties.


```C++
void DisplayDeviceInformation(IEnumMoniker *pEnum)
{
    IMoniker *pMoniker = NULL;

    while (pEnum->Next(1, &amp;pMoniker, NULL) == S_OK)
    {
        IPropertyBag *pPropBag;
        HRESULT hr = pMoniker->BindToStorage(0, 0, IID_PPV_ARGS(&amp;pPropBag));
        if (FAILED(hr))
        {
            pMoniker->Release();
            continue;  
        } 

        VARIANT var;
        VariantInit(&amp;var);

        // Get description or friendly name.
        hr = pPropBag->Read(L"Description", &amp;var, 0);
        if (FAILED(hr))
        {
            hr = pPropBag->Read(L"FriendlyName", &amp;var, 0);
        }
        if (SUCCEEDED(hr))
        {
            printf("%S\n", var.bstrVal);
            VariantClear(&amp;var); 
        }

        hr = pPropBag->Write(L"FriendlyName", &amp;var);

        // WaveInID applies only to audio capture devices.
        hr = pPropBag->Read(L"WaveInID", &amp;var, 0);
        if (SUCCEEDED(hr))
        {
            printf("WaveIn ID: %d\n", var.lVal);
            VariantClear(&amp;var); 
        }

        hr = pPropBag->Read(L"DevicePath", &amp;var, 0);
        if (SUCCEEDED(hr))
        {
            // The device path is not intended for display.
            printf("Device path: %S\n", var.bstrVal);
            VariantClear(&amp;var); 
        }

        pPropBag->Release();
        pMoniker->Release();
    }
}

void main()
{
    HRESULT hr = CoInitializeEx(NULL, COINIT_MULTITHREADED);
    if (SUCCEEDED(hr))
    {
        IEnumMoniker *pEnum;

        hr = EnumerateDevices(CLSID_VideoInputDeviceCategory, &amp;pEnum);
        if (SUCCEEDED(hr))
        {
            DisplayDeviceInformation(pEnum);
            pEnum->Release();
        }
        hr = EnumerateDevices(CLSID_AudioInputDeviceCategory, &amp;pEnum);
        if (SUCCEEDED(hr))
        {
            DisplayDeviceInformation(pEnum);
            pEnum->Release();
        }
        CoUninitialize();
    }
}
```



To create a DirectShow capture filter for the device, call the [**IMoniker::BindToObject**](com.imoniker_bindtoobject) method to get an [**IBaseFilter**](ibasefilter.md) pointer. Then call [**IFilterGraph::AddFilter**](ifiltergraph-addfilter.md) to add the filter to the filter graph:


```C++
IBaseFilter *pCap = NULL;
hr = pMoniker->BindToObject(0, 0, IID_IBaseFilter, (void**)&amp;pCap);
if (SUCCEEDED(hr))
{
    hr = m_pGraph->AddFilter(pCap, L"Capture Filter");
}
```



## Related topics

<dl> <dt>

[Audio Capture](audio-capture.md)
</dt> <dt>

[Video Capture](video-capture.md)
</dt> </dl>

 

 


