﻿---
Description: 'Specifies the start time for presentations that are queued after the first presentation.'
ms.assetid: '087f5d61-b3e6-4fdf-98e6-b018de7b237f'
title: 'MF\_TOPOLOGY\_START\_TIME\_ON\_PRESENTATION\_SWITCH attribute'
---

# MF\_TOPOLOGY\_START\_TIME\_ON\_PRESENTATION\_SWITCH attribute

Specifies the start time for presentations that are queued after the first presentation.

## Data type

**INT64** stored as **UINT64**

## Get/set

To get this attribute, call [**IMFAttributes::GetUINT64**](imfattributes-getuint64.md).

To set this attribute, call [**IMFAttributes::SetUINT64**](imfattributes-setuint64.md).

## Applies To

[**IMFTopology**](imftopology.md)

## Remarks

When the application queues the first presentation on the Media Session, the application specifies the start time in the *pvarStartPosition* parameter of the [**IMFMediaSession::Start**](imfmediasession-start.md) method. For any subsequent presentations, however, the start time is given by the MF\_TOPOLOGY\_START\_TIME\_ON\_PRESENTATION\_SWITCH attribute on the topology. The start time is specified in 100-nanosecond units, relative to the beginning of the presentation. For example, if the value is 50000000, playback starts 5 seconds into the presentation. If this attribute is not set, the default start time is zero.

The GUID constant for this attribute is exported from mfuuid.lib.

## Requirements



|                                     |                                                                                    |
|-------------------------------------|------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 7 \[desktop apps only\]<br/>                                         |
| Minimum supported server<br/> | Windows Server 2008 R2 \[desktop apps only\]<br/>                            |
| Header<br/>                   | <dl> <dt>Mfidl.h</dt> </dl> |



## See also

<dl> <dt>

[Alphabetical List of Media Foundation Attributes](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Topology Attributes](topology-attributes.md)
</dt> </dl>

 

 



