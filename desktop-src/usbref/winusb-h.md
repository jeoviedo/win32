---
Description: 'This section contains reference topics for the Winusb.h header.'
ms.assetid: '21D5E634-7437-4620-8440-9134EDF9CF98'
title: 'Winusb.h'
---

# Winusb.h

This section contains reference topics for the Winusb.h header. This header contains programming interfaces that are exposed by the Microsoft-provided USB driver stack.

> [!Note]  
> WinUSB functions require Windows XP or later. You can use these functions in your C/C++ application to communicate with your USB device. Microsoft does not provide a managed API for WinUSB

�

## In this section



| Topic                                                                                        | Description                                                                                                                                                                                                                                                              |
|----------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**WinUsb\_AbortPipe**](winusb-abortpipe.md)<br/>                                     | The [**WinUsb\_AbortPipe**](winusb-abortpipe.md) function aborts all of the pending transfers for a pipe. This is a synchronous operation.<br/>                                                                                                                   |
| [**WinUsb\_ControlTransfer**](winusb-controltransfer.md)<br/>                         | The [**WinUsb\_ControlTransfer**](winusb-controltransfer.md) function transmits control data over a default control endpoint.<br/>                                                                                                                                |
| [**WinUsb\_FlushPipe**](winusb-flushpipe.md)<br/>                                     | The **WinUsb\_FlushPipe** function discards any data that is cached in a pipe. This is a synchronous operation.<br/>                                                                                                                                               |
| [**WinUsb\_Free**](winusb-free.md)<br/>                                               | The [**WinUsb\_Free**](winusb-free.md) function releases all of the resources that [**WinUsb\_Initialize**](winusb-initialize.md) allocated. This is a synchronous operation.<br/>                                                                               |
| [**WinUsb\_GetAdjustedFrameNumber**](winusb-getadjustedframenumber.md)<br/>           | The [**WinUsb\_GetAdjustedFrameNumber**](winusb-getadjustedframenumber.md) function computes what the current USB frame number should be based on the frame number value and timestamp. <br/>                                                                     |
| [**WinUsb\_GetAssociatedInterface**](winusb-getassociatedinterface.md)<br/>           | The [**WinUsb\_GetAssociatedInterface**](winusb-getassociatedinterface.md) function retrieves a handle for an associated interface. This is a synchronous operation.<br/>                                                                                         |
| [**WinUsb\_GetCurrentFrameNumber**](winusb-getcurrentframenumber.md)<br/>             | The [**WinUsb\_GetCurrentFrameNumber**](winusb-getcurrentframenumber.md) function gets the current frame number for the bus.<br/>                                                                                                                                 |
| [**WinUsb\_GetCurrentFrameNumberAndQpc**](winusb-getcurrentframenumberandqpc.md)<br/> | The [**WinUsb\_GetCurrentFrameNumberAndQpc**](winusb-getcurrentframenumberandqpc.md) function retrieves the system query performance counter (QPC) value synchronized with the frame and microframe.<br/>                                                         |
| [**WinUsb\_GetCurrentAlternateSetting**](winusb-getcurrentalternatesetting.md)<br/>   | The [**WinUsb\_GetCurrentAlternateSetting**](winusb-getcurrentalternatesetting.md) function gets the current alternate interface setting for an interface. This is a synchronous operation.<br/>                                                                  |
| [**WinUsb\_GetDescriptor**](winusb-getdescriptor.md)<br/>                             | The [**WinUsb\_GetDescriptor**](winusb-getdescriptor.md) function returns the requested descriptor. This is a synchronous operation.<br/>                                                                                                                         |
| [**WinUsb\_GetOverlappedResult**](winusb-getoverlappedresult.md)<br/>                 | The **WinUsb\_GetOverlappedResult** function retrieves the results of an overlapped operation on the specified file.<br/>                                                                                                                                          |
| [**WinUsb\_GetPipePolicy**](winusb-getpipepolicy.md)<br/>                             | The [**WinUsb\_GetPipePolicy**](winusb-getpipepolicy.md) function retrieves the policy for a specific pipe associated with an endpoint on the device. This is a synchronous operation.<br/>                                                                       |
| [**WinUsb\_GetPowerPolicy**](winusb-getpowerpolicy.md)<br/>                           | The [**WinUsb\_GetPowerPolicy**](winusb-getpowerpolicy.md) function retrieves the power policy for a device. This is a synchronous operation.<br/>                                                                                                                |
| [**WinUsb\_Initialize**](winusb-initialize.md)<br/>                                   | The [**WinUsb\_Initialize**](winusb-initialize.md) function creates a WinUSB handle for the device specified by a file handle.<br/>                                                                                                                               |
| [**WinUsb\_QueryDeviceInformation**](winusb-querydeviceinformation.md)<br/>           | The [**WinUsb\_QueryDeviceInformation**](winusb-querydeviceinformation.md) function gets information about the physical device that is associated with a WinUSB interface handle.<br/>                                                                            |
| [**WinUsb\_QueryInterfaceSettings**](winusb-queryinterfacesettings.md)<br/>           | The [**WinUsb\_QueryInterfaceSettings**](winusb-queryinterfacesettings.md) function retrieves the interface descriptor for the specified alternate interface settings for a particular interface handle.<br/>                                                     |
| [**WinUsb\_QueryPipe**](winusb-querypipe.md)<br/>                                     | The [**WinUsb\_QueryPipe**](winusb-querypipe.md) function retrieves information about the specified endpoint and the associated pipe for an interface.<br/>                                                                                                       |
| [**WinUsb\_QueryPipeEx**](winusb-querypipeex.md)<br/>                                 | The [**WinUsb\_QueryPipeEx**](winusb-querypipeex.md) function retrieves extended information about the specified endpoint and the associated pipe for an interface.<br/>                                                                                          |
| [**WinUsb\_ReadIsochPipe**](winusb-readisochpipe.md)<br/>                             | The [**WinUsb\_ReadIsochPipe**](winusb-readisochpipe.md) function reads data from an isochronous OUT endpoint. <br/>                                                                                                                                              |
| [**WinUsb\_ReadIsochPipeAsap**](winusb-readisochpipeasap.md)<br/>                     | The [**WinUsb\_ReadIsochPipeAsap**](winusb-readisochpipeasap.md) function submits a request that reads data from an isochronous OUT endpoint. <br/>                                                                                                               |
| [**WinUsb\_ReadPipe**](winusb-readpipe.md)<br/>                                       | The [**WinUsb\_ReadPipe**](winusb-readpipe.md) function reads data from the specified pipe.<br/>                                                                                                                                                                  |
| [**WinUsb\_RegisterIsochBuffer**](winusb-registerisochbuffer.md)<br/>                 | The [**WinUsb\_RegisterIsochBuffer**](winusb-registerisochbuffer.md) function registers a buffer to be used for isochronous transfers.<br/>                                                                                                                       |
| [**WinUsb\_ResetPipe**](winusb-resetpipe.md)<br/>                                     | The [**WinUsb\_ResetPipe**](winusb-resetpipe.md) function resets the data toggle and clears the stall condition on a pipe.<br/>                                                                                                                                   |
| [**WinUsb\_SetCurrentAlternateSetting**](winusb-setcurrentalternatesetting.md)<br/>   | The [**WinUsb\_SetCurrentAlternateSetting**](winusb-setcurrentalternatesetting.md) function sets the alternate setting of an interface.<br/>                                                                                                                      |
| [**WinUsb\_SetPipePolicy**](winusb-setpipepolicy.md)<br/>                             | The [**WinUsb\_SetPipePolicy**](winusb-setpipepolicy.md) function sets the policy for a specific pipe associated with an endpoint on the device. This is a synchronous operation.<br/>                                                                            |
| [**WinUsb\_SetPowerPolicy**](winusb-setpowerpolicy.md)<br/>                           | The [**WinUsb\_SetPowerPolicy**](winusb-setpowerpolicy.md) function sets the power policy for a device.<br/>                                                                                                                                                      |
| [**WinUsb\_StartTrackingForTimeSync**](winusb-starttrackingfortimesync.md)<br/>       | The [**WinUsb\_StartTrackingForTimeSync**](winusb-starttrackingfortimesync.md) function starts the time synchronization feature in the USB driver stack that gets the associated system QPC time for USB bus frames and microframes. <br/>                        |
| [**WinUsb\_StopTrackingForTimeSync**](winusb-stoptrackingfortimesync.md)<br/>         | The [**WinUsb\_StopTrackingForTimeSync**](winusb-stoptrackingfortimesync.md) function tops the time synchronization feature in the USB driver stack that gets the associated system QPC time for USB bus frames and microframes. <br/>                            |
| [**WINUSB\_SETUP\_PACKET**](winusb-setup-packet.md)<br/>                              | The [**WINUSB\_SETUP\_PACKE**](winusb-setup-packet.md)T structure describes a USB setup packet.<br/>                                                                                                                                                              |
| [**WinUsb\_UnregisterIsochBuffer**](winusb-unregisterisochbuffer.md)<br/>             | The [**WinUsb\_UnregisterIsochBuffer**](winusb-unregisterisochbuffer.md) function releases all of the resources that [**WinUsb\_RegisterIsochBuffer**](winusb-registerisochbuffer.md) allocated for isochronous transfers. This is a synchronous operation.<br/> |
| [**WinUsb\_WriteIsochPipe**](winusb-writeisochpipe.md)<br/>                           | The [**WinUsb\_WriteIsochPipe**](winusb-writeisochpipe.md) function writes the contents of a caller-supplied buffer to an isochronous OUT endpoint, starting on a specified frame number. <br/>                                                                   |
| [**WinUsb\_WriteIsochPipeAsap**](winusb-writeisochpipeasap.md)<br/>                   | The [**WinUsb\_WriteIsochPipeAsap**](winusb-writeisochpipeasap.md) submits a request for writing the contents of a buffer to an isochronous OUT endpoint. <br/>                                                                                                   |
| [**WinUsb\_WritePipe**](winusb-writepipe.md)<br/>                                     | The [**WinUsb\_WritePipe**](winusb-writepipe.md) function writes data to a pipe.<br/>                                                                                                                                                                             |



�

�

�

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Busbref\buses%5D:%20Winusb.h%20%20RELEASE:%20%285/17/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")



