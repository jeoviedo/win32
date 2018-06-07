---
Description: The get\_ScaleY method retrieves the amount by which the wipe is stretched vertically.
ms.assetid: d8b80f19-2ec5-4d66-bd13-d6f7b5144345
title: IDxtJpeg::get\_ScaleY method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IDxtJpeg::get\_ScaleY method

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

The `get_ScaleY` method retrieves the amount by which the wipe is stretched vertically.

## Syntax


```C++
HRESULT get_ScaleY(
  [out, retval] long *pVal
);
```



## Parameters

<dl> <dt>

*pVal* \[out, retval\]
</dt> <dd>

Receives the amount by which the wipe is stretched vertically, as a percentage of the original wipe definition. For example, the value 1.0 means no stretching, and 2.0 means 200% stretching.

</dd> </dl>

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

> [!Note]  
> The header file Qedit.h is not compatible with Direct3D headers later than version 7.

 

> [!Note]  
> To obtain Qedit.h, download the [Microsoft Windows SDK Update for Windows Vista and .NET Framework 3.0](http://go.microsoft.com/fwlink/p/?linkid=129787). Qedit.h is not available in the Microsoft Windows SDK for Windows 7 and .NET Framework 3.5 Service Pack 1.

 

## Requirements



|                    |                                                                                         |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Qedit.h</dt> </dl>      |
| Library<br/> | <dl> <dt>Strmiids.lib</dt> </dl> |



## See also

<dl> <dt>

[**IDxtJpeg Interface**](idxtjpeg.md)
</dt> </dl>

 

 



