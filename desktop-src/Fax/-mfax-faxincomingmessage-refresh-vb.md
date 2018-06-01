---
Description: Refreshes FaxIncomingMessage object information from the fax server.
ms.assetid: 7c07853e-a883-41d3-86ba-fc832c0b8300
title: FaxIncomingMessage.Refresh method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# FaxIncomingMessage.Refresh method

Refreshes [**FaxIncomingMessage**](-mfax-faxincomingmessage.md) object information from the fax server. When the **Refresh** method is called, any configuration changes made after the last [**Save**](-mfax-faxincomingmessage-save-vb.md) method call are lost, except for the properties that are committed with the [**Reassign**](-mfax-faxincomingmessage-reassign-vb.md) method: [**Subject**](-mfax-faxincomingmessage-subject-vb.md), [**SenderName**](-mfax-faxincomingmessage-sendername-vb.md), [**SenderFaxNumber**](-mfax-faxincomingmessage-senderfaxnumber-vb.md), and [**HasCoverPage**](-mfax-faxincomingmessage-hascoverpage-vb.md).

> [!Note]  
> This method is supported only in Windows Vista and later.

 

## Syntax


```VB
FaxIncomingMessage.Refresh() As Long
```



## Parameters

This method has no parameters.

## Remarks

To use this method, a user must have the [****far2QUERY\_CONFIG****](/previous-versions/windows/desktop/api/FaxComex/ne-faxcomex-fax_access_rights_enum_2) access rights.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                    |
| Header<br/>                   | <dl> <dt>FaxComex.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Fxscomex.dll</dt> </dl> |



## See also

<dl> <dt>

[**FaxIncomingMessage**](-mfax-faxincomingmessage.md)
</dt> <dt>

[**IFaxIncomingMessage2**](/previous-versions/windows/desktop/api/FaxComex/nn-faxcomex-ifaxincomingmessage2)
</dt> </dl>

 

 



