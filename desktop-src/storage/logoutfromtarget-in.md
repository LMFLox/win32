---
title: LogoutFromTarget\_IN structure
description: The LogoutFromTarget\_IN structure holds the input data for the LogoutFromTarget method, which is used to log out from an iSCSI target.
ms.assetid: 'a52d5995-1fb7-4b73-9d3f-c945e7219a49'
keywords: ["LogoutFromTarget_IN structure Storage Devices", "PLogoutFromTarget_IN structure pointer Storage Devices"]
topic_type:
- apiref
api_name:
- LogoutFromTarget_IN
api_location:
- iscsiop.h
api_type:
- HeaderDef
---

# LogoutFromTarget\_IN structure

The LogoutFromTarget\_IN structure holds the input data for the [LogoutFromTarget](https://msdn.microsoft.com/library/windows/hardware/ff561602) method, which is used to log out from an iSCSI target.

## Syntax


```C++
typedef struct _LogoutFromTarget_IN {
  ULONGLONG UniqueSessionId;
} LogoutFromTarget_IN, *PLogoutFromTarget_IN;
```



## Members

<dl> <dt>

**UniqueSessionId**
</dt> <dd>

A 64-bit integer that uniquely identifies the session. The [LoginToTarget](https://msdn.microsoft.com/library/windows/hardware/ff561599) and [AddConnectionToSession](https://msdn.microsoft.com/library/windows/hardware/ff550121) methods both return this value in the *UniqueSessionId* parameter. Do not confuse this value with the values in the ISID and TSID members.

</dd> </dl>

## Remarks

You must implement this method.

## Requirements



|                   |                                                                                                          |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>Iscsiop.h (include Iscsiop.h)</dt> </dl> |



## See also

<dl> <dt>

[AddConnectionToSession](https://msdn.microsoft.com/library/windows/hardware/ff550121)
</dt> <dt>

[LoginToTarget](https://msdn.microsoft.com/library/windows/hardware/ff561599)
</dt> <dt>

[**LogoutFromTarget\_OUT**](logoutfromtarget-out.md)
</dt> <dt>

[MSiSCSI\_Operations WMI Class](https://msdn.microsoft.com/library/windows/hardware/ff563091)
</dt> </dl>

�

�

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bstorage\storage%5D:%20LogoutFromTarget_IN%20structure%20%20RELEASE:%20%283/29/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





