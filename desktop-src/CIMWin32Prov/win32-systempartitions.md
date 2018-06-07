---
Description: The Win32\_SystemPartitions association WMI class relates a computer system and a disk partition on that system.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: e8f02cd0-9446-4258-b476-5dc6c72c80d4
ms.prod: windows-server-dev
ms.technology:
- cimwin32
- windows-management-instrumentation
ms.tgt_platform: multiple
title: Win32\_SystemPartitions class
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Win32\_SystemPartitions class

The **Win32\_SystemPartitions** association [WMI class](https://msdn.microsoft.com/cfe4bcca-692e-45cd-a840-93ebfe4ae267) relates a computer system and a disk partition on that system.

The following syntax is simplified from Managed Object Format (MOF) code and includes all of the inherited properties. Properties and methods are in alphabetic order, not MOF order.

## Syntax

``` syntax
[Dynamic, Provider("CIMWin32"), UUID("{8502C4F5-5FBB-11D2-AAC1-006008C78BC7}"), AMENDMENT]
class Win32_SystemPartitions : Win32_SystemDevices
{
  Win32_ComputerSystem REF GroupComponent;
  Win32_DiskPartition  REF PartComponent;
};
```

## Members

The **Win32\_SystemPartitions** class has these types of members:

-   [Properties](#properties)

### Properties

The **Win32\_SystemPartitions** class has these properties.

<dl> <dt>

**GroupComponent**
</dt> <dd> <dl> <dt>

Data type: **Win32\_ComputerSystem**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/671ea769-f68d-4788-96f5-c4f86ab3b00e) ("GroupComponent"), [**MappingStrings**](https://msdn.microsoft.com/671ea769-f68d-4788-96f5-c4f86ab3b00e) ("WMI\|Win32\_ComputerSystem")
</dt> </dl>

Reference to the instance representing the properties of the computer system where the disk partition is located.

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Data type: **Win32\_DiskPartition**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/671ea769-f68d-4788-96f5-c4f86ab3b00e) ("PartComponent"), [**MappingStrings**](https://msdn.microsoft.com/671ea769-f68d-4788-96f5-c4f86ab3b00e) ("WMI\|Win32\_DiskPartition")
</dt> </dl>

Reference to the instance representing the properties of a disk partition that exists on the computer system.

</dd> </dl>

## Remarks

The **Win32\_SystemPartitions** class is derived from [**Win32\_SystemDevices**](win32-systemdevices.md).

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista<br/>                                                                |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                          |
| Namespace<br/>                | Root\\CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## See also

<dl> <dt>

[**Win32\_SystemDevices**](win32-systemdevices.md)
</dt> <dt>

[Operating System Classes](https://www.bing.com/search?q=Operating+System+Classes)
</dt> </dl>

 

 



