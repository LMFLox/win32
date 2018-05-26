---
Description: This section contains reference topics for the Mmddk.h header.
ms.assetid: 0D2FBECF-7A50-4C72-A55E-7E1CCBC5F3FB
title: Mmddk.h
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Mmddk.h

This section contains reference topics for the Mmddk.h header.

## In this section



| Topic                                                                                    | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**DRV\_QUERYDEVICEINTERFACE**](/windows/win32/mmddk/?branch=master)<br/>                 | The DRV\_QUERYDEVICEINTERFACE message queries for the device-interface name of a **waveIn**, **waveOut**, **midiIn**, **midiOut**, or **mixer** device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [**DRV\_QUERYDEVICEINTERFACESIZE**](/windows/win32/mmddk/?branch=master)<br/>         | The DRV\_QUERYDEVICEINTERFACESIZE message queries for the size of the buffer required to hold the device-interface name.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| [**DRV\_QUERYDEVNODE**](/windows/win32/mmddk/?branch=master)<br/>                                 | The DRV\_QUERYDEVNODE message queries for the [devnode](wdkgloss.d#wdkgloss-devnode) number assigned to the device by the Plug and Play manager.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**DRV\_QUERYMAPPABLE**](/windows/win32/mmddk/?branch=master)<br/>                               | The DRV\_QUERYMAPPABLE message queries for whether the specified device can be used by a mapper.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| [**DRVM\_MAPPER\_CONSOLEVOICECOM\_GET**](/windows/win32/mmddk/?branch=master)<br/> | The DRVM\_MAPPER\_CONSOLEVOICECOM\_GET message retrieves the device ID of the preferred voice-communications device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**DRVM\_MAPPER\_PREFERRED\_GET**](/windows/win32/mmddk/?branch=master)<br/>             | The DRVM\_MAPPER\_PREFERRED\_GET message retrieves the device ID of the preferred audio device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [**MDEVICECAPSEX**](/windows/win32/mmddk/ns-mmddk-mdevicecapsex?branch=master)<br/>                                        | The `MDEVICECAPSEX` structure contains device capability information for Plug and Play (PnP) device drivers.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| [**MIDIOPENDESC**](/windows/win32/mmddk/ns-mmddk-midiopendesc_tag?branch=master)<br/>                                          | The `MIDIOPENDESC` structure is a client-filled structure that provides information about how to open a MIDI device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**MODM\_CACHEDRUMPATCHES**](/windows/win32/Mmddk/?branch=master)<br/>                       | WINMM sends the `MODM_CACHEDRUMPATCHES` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to ask the driver to cache or uncache the specified drum keys. This allows the internal synthesizer drivers to load the patches that are needed by the client application.<br/>                                                                                                                                                                                                                                                                               |
| [**MODM\_CACHEPATCHES**](/windows/win32/Mmddk/?branch=master)<br/>                               | WINMM sends the `MODM_CACHEPATCHES` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to request that the driver cache or uncache the specified patches. This allows internal synthesizer drivers to load the patches that are needed by a client application.<br/>                                                                                                                                                                                                                                                                                     |
| [**MODM\_DATA**](/windows/win32/Mmddk/?branch=master)<br/>                                               | MMSYSTEM sends the `MODM_DATA` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver when the client wants to make a single MIDI event available as output.<br/>                                                                                                                                                                                                                                                                                                                                                                                            |
| [**MODM\_GETDEVCAPS**](/windows/win32/Mmddk/?branch=master)<br/>                                   | WINMM sends the `MODM_GETDEVCAPS` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to retrieve information about the capabilities of a specific MIDI output device.<br/>                                                                                                                                                                                                                                                                                                                                                                               |
| [**MODM\_GETNUMDEVS**](/windows/win32/Mmddk/?branch=master)<br/>                                   | WINMM sends the `MODM_GETNUMDEVS` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to request the number of MIDI output devices available.<br/>                                                                                                                                                                                                                                                                                                                                                                                                        |
| [**MODM\_GETPOS**](/windows/win32/Mmddk/?branch=master)<br/>                                           | WINMM sends the `MODM_GETPOS` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to request the current position of the stream pointer in the data stream.<br/>                                                                                                                                                                                                                                                                                                                                                                                          |
| [**MODM\_GETVOLUME**](/windows/win32/Mmddk/?branch=master)<br/>                                     | WINMM sends the `MODM_GETVOLUME` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to request the current volume level setting for a MIDI device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                  |
| [**MODM\_LONGDATA**](/windows/win32/Mmddk/?branch=master)<br/>                                       | WINMM sends the `MODM_LONGDATA` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver when a client application wants the driver to make a data block available as output. This data block typically contains one or more MIDI events, including system-exclusive events. If the data block contains more than one MIDI event, the events are packed into the data block with no padding.<br/> If a client of the MIDI output driver wants to send a single MIDI event, it is more efficient to use the [**MODM\_DATA**](/windows/win32/Mmddk/?branch=master) message.<br/> |
| [**MODM\_OPEN**](/windows/win32/Mmddk/?branch=master)<br/>                                               | WINMM sends the `MODM_OPEN` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to allocate a specified device that a client application can use.<br/>                                                                                                                                                                                                                                                                                                                                                                                                    |
| [**MODM\_PAUSE**](/windows/win32/Mmddk/?branch=master)<br/>                                             | WINMM sends the `MODM_PAUSE` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to temporarily pause output requests. Playback of streams stops but no buffers are marked as done.<br/>                                                                                                                                                                                                                                                                                                                                                                  |
| [**MODM\_PREPARE**](/windows/win32/Mmddk/?branch=master)<br/>                                         | WINMM sends the `MODM_PREPARE` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to request that the driver configure a system-exclusive data block for output. If data blocks are accessed at interrupt time, they must be page-locked to ensure that the memory is not swapped out to disk.<br/>                                                                                                                                                                                                                                                      |
| [**MODM\_PROPERTIES**](/windows/win32/Mmddk/?branch=master)<br/>                                   | WINMM sends the `MODM_PROPERTIES` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to change the properties of the output stream.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**MODM\_RESET**](/windows/win32/Mmddk/?branch=master)<br/>                                             | WINMM sends the `MODM_RESET` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to stop output from the output queue and to turn off any notes that are playing.<br/>                                                                                                                                                                                                                                                                                                                                                                                    |
| [**MODM\_RESTART**](/windows/win32/Mmddk/?branch=master)<br/>                                         | WINMM sends the `MODM_RESTART` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to restart playback after a [**MODM\_PAUSE**](/windows/win32/Mmddk/?branch=master).<br/>                                                                                                                                                                                                                                                                                                                                                                                                    |
| [**MODM\_SETVOLUME**](/windows/win32/Mmddk/?branch=master)<br/>                                     | WINMM sends the `MODM_SETVOLUME` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to set the volume for a MIDI device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                            |
| [**MODM\_STOP**](/windows/win32/Mmddk/?branch=master)<br/>                                               | WINMM sends the `MODM_STOP` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to stop output from the output queue and to turn off any notes that are playing.<br/>                                                                                                                                                                                                                                                                                                                                                                                     |
| [**MODM\_STRMDATA**](/windows/win32/Mmddk/?branch=master)<br/>                                       | WINMM sends the `MODM_STRMDATA` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to get the MIDI output device to send stream data.<br/>                                                                                                                                                                                                                                                                                                                                                                                                               |
| [**MODM\_UNPREPARE**](/windows/win32/Mmddk/?branch=master)<br/>                                     | WINMM sends the `MODM_UNPREPARE` message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver to clean up the memory segment that was configured by [**MODM\_PREPARE**](/windows/win32/Mmddk/?branch=master).<br/>                                                                                                                                                                                                                                                                                                                                                                    |
| [**MOM\_CLOSE**](/windows/win32/Mmddk/?branch=master)<br/>                                               | WINMM sends the [**MOM\_CLOSE**](/windows/win32/Mmddk/?branch=master) message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver in response to a call from a client application.<br/>                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**MOM\_DONE**](/windows/win32/Mmsystem/?branch=master)<br/>                                                 | WINMM sends the [**MOM\_DONE**](/windows/win32/Mmsystem/?branch=master) message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of MIDI output driver, to return a system-exclusive data block to the client application.<br/>                                                                                                                                                                                                                                                                                                                                                                                  |
| [**MOM\_OPEN**](/windows/win32/Mmddk/?branch=master)<br/>                                                 | WINMM sends the [**MOM\_OPEN**](/windows/win32/Mmddk/?branch=master) message to the [**modMessage**](/windows/win32/mmddk/?branch=master) function of a MIDI output driver.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                   |



 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Baudio\audio%5D:%20Mmddk.h%20%20RELEASE:%20%285/12/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")



