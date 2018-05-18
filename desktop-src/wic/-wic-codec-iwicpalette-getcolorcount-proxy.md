---
Description: 'Proxy function for the GetColorCount method.'
ms.assetid: '2ad87383-4d30-4df0-b43a-95fdad1d59f9'
title: 'IWICPalette\_GetColorCount\_Proxy function'
---

# IWICPalette\_GetColorCount\_Proxy function

Proxy function for the [**GetColorCount**](-wic-codec-iwicpalette-getcolorcount.md) method.

## Syntax


```C++
HRESULT IWICPalette_GetColorCount_Proxy(
  _In_��IWICPalette *THIS_PTR,
  _Out_�UINT �������*pcCount
);
```



## Parameters

<dl> <dt>

*THIS\_PTR* \[in\]
</dt> <dd>

Type: **[**IWICPalette**](-wic-codec-iwicpalette.md)\***

Pointer to this [**IWICPalette**](-wic-codec-iwicpalette.md) object.

</dd> <dt>

*pcCount* \[out\]
</dt> <dd>

Type: **UINT\***

Pointer that receives the number of colors in the color table.

</dd> </dl>

## Return value

Type: **HRESULT**

If this function succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

## Requirements



|                                     |                                                                                                                                                                  |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP with SP2, Windows�Vista \[desktop apps only\]<br/>                                                                                              |
| Minimum supported server<br/> | Windows Server�2008 \[desktop apps only\]<br/>                                                                                                             |
| DLL<br/>                      | <dl> <dt>Windowscodecs.dll; </dt> <dt>Wincodec.lib</dt> </dl> |



�

�



