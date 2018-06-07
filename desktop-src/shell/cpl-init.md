---
Description: Sent to the CPlApplet function of a Control Panel application to prompt it to perform global initialization, especially memory allocation.
ms.assetid: 0e7e9b14-9f44-496e-a518-5d3ae92868c5
title: CPL\_INIT message
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CPL\_INIT message

Sent to the [**CPlApplet**](/windows/desktop/api/Cpl/nc-cpl-applet_proc) function of a Control Panel application to prompt it to perform global initialization, especially memory allocation.


```C++

                CPlApplet(

    hwndCPl,

    CPL_INIT,

    wParam,  // = 0; not used, must be zero

    lParam   // = 0; not used, must be zero 

);

            
```



## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>Must be zero.</dd> <dt>

*lParam* 
</dt> <dd>Must be zero.</dd> </dl>

## Return value

If initialization succeeds, the [**CPlApplet**](/windows/desktop/api/Cpl/nc-cpl-applet_proc) function should return nonzero. Otherwise, it should return zero.

If [**CPlApplet**](/windows/desktop/api/Cpl/nc-cpl-applet_proc) returns zero, the controlling application ends communication and releases the DLL containing the Control Panel application.

## Remarks

Because this is the only way a Control Panel application can signal an error condition, the application should allocate memory in response to this message.

This message is sent immediately after the DLL containing the application is loaded.

## Requirements



|                                     |                                                                                  |
|-------------------------------------|----------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                      |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                             |
| Header<br/>                   | <dl> <dt>Cpl.h</dt> </dl> |



## See also

<dl> <dt>

[**FreeLibrary**](https://msdn.microsoft.com/823d3147-4ba8-4fe5-ade4-e5604f47eb0a)
</dt> </dl>

 

 



