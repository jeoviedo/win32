---
title: AddNamespaceFolderTarget method of the MSFT\_DfsNamespaceFolderTarget class
description: Adds a new target for a DFS folder.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: '16c7ecc0-46a3-40d7-8e58-a5c3755b3961'
ms.prod: 'windows-server-dev'
ms.technology:
- 'distributed-file-system-namespace'
- 'windows-management-instrumentation'
ms.tgt_platform: multiple
keywords: ["AddNamespaceFolderTarget method", "AddNamespaceFolderTarget method, MSFT_DfsNamespaceFolderTarget class", "MSFT_DfsNamespaceFolderTarget class, AddNamespaceFolderTarget method"]
topic_type:
- apiref
api_name:
- MSFT_DfsNamespaceFolderTarget.AddNamespaceFolderTarget
api_location:
- DfsNCimProv.dll
api_type:
- COM
---

# AddNamespaceFolderTarget method of the MSFT\_DfsNamespaceFolderTarget class

Adds a new target for a DFS folder.

## Syntax


```mof
uint32 AddNamespaceFolderTarget(
  [in]��string �����������������������NamespacePath,
  [in]��string �����������������������TargetPath,
  [in]��uint32 �����������������������State,
  [in]��uint32 �����������������������ReferralPriorityRank,
  [in]��sint32 �����������������������ReferralPriorityClass,
  [out]�MSFT_DfsNamespaceFolderTarget cmdletOutput
);
```



## Parameters

<dl> <dt>

*NamespacePath* \[in\]
</dt> <dd>

The Universal Naming Convention (UNC) path of the DFS folder for which to create a new target.

</dd> <dt>

*TargetPath* \[in\]
</dt> <dd>

The UNC path of a DFS folder to be set as the new target for the DFS folder. If the path does not already exist, the method creates a new folder for that path to become the new target.

</dd> <dt>

*State* \[in\]
</dt> <dd>

The state of the target of a DFS folder.

<dt>

<span id="OFFLINE"></span><span id="offline"></span>

<span id="OFFLINE"></span><span id="offline"></span>**OFFLINE** (3)


</dt> <dd>

Not online. Referrals are disabled.

</dd> <dt>

<span id="ONLINE"></span><span id="online"></span>

<span id="ONLINE"></span><span id="online"></span>**ONLINE** (4)


</dt> <dd>

Online. Referrals are enabled.

</dd> </dl> </dd> <dt>

*ReferralPriorityRank* \[in\]
</dt> <dd>

The priority rank of the target of a DFS folder.

</dd> <dt>

*ReferralPriorityClass* \[in\]
</dt> <dd>

The priority class of the target of a DFS folder.

<dt>

<span id="Invalid"></span><span id="invalid"></span><span id="INVALID"></span>

<span id="Invalid"></span><span id="invalid"></span><span id="INVALID"></span>**Invalid** (-1)


</dt> <dd>

Invalid priority.

</dd> <dt>

<span id="Normal"></span><span id="normal"></span><span id="NORMAL"></span>

<span id="Normal"></span><span id="normal"></span><span id="NORMAL"></span>**Normal** (0)


</dt> <dd>

Site cost, normal priority.

</dd> <dt>

<span id="global-high"></span><span id="GLOBAL-HIGH"></span>

<span id="global-high"></span><span id="GLOBAL-HIGH"></span>**global-high** (1)


</dt> <dd>

Global, high priority.

</dd> <dt>

<span id="sitecost-high"></span><span id="SITECOST-HIGH"></span>

<span id="sitecost-high"></span><span id="SITECOST-HIGH"></span>**sitecost-high** (2)


</dt> <dd>

Site cost, high priority.

</dd> <dt>

<span id="sitecost-low"></span><span id="SITECOST-LOW"></span>

<span id="sitecost-low"></span><span id="SITECOST-LOW"></span>**sitecost-low** (3)


</dt> <dd>

Site cost, low priority.

</dd> <dt>

<span id="global-low"></span><span id="GLOBAL-LOW"></span>

<span id="global-low"></span><span id="GLOBAL-LOW"></span>**global-low** (4)


</dt> <dd>

Global, low priority.

</dd> </dl> </dd> <dt>

*cmdletOutput* \[out\]
</dt> <dd>

When this method returns, contains output from the **New-DFSNamespaceFolderTarget** cmdlet. This parameter is passed uninitialized.

</dd> </dl>

## Remarks

The *NamespacePath* and *TargetPath* parameters have a format of \\\\HostName\\SharedName\[\\ObjectName\]\*, where:

-   The HostName component represents either the host name of a server or the domain name of a domain that hosts resources.
-   The SharedName component represents the share name or the name of the resource that is being accessed.
-   Each ObjectName component represents the name of a directory on the resource that is being accessed.

## Requirements



|                                     |                                                                                            |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                  |
| Minimum supported server<br/> | Windows Server�2012<br/>                                                             |
| Namespace<br/>                | Root\\Microsoft\\Windows\\dfsn<br/>                                                  |
| MOF<br/>                      | <dl> <dt>DfsNCimProv.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>DfsNCimProv.dll</dt> </dl> |



## See also

<dl> <dt>

[**MSFT\_DfsNamespaceFolderTarget**](msft-dfsnamespacefoldertarget.md)
</dt> </dl>

�

�




