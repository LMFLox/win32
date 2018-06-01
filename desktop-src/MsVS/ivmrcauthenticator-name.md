---
title: IVMRCAuthenticator Name property
description: The Name property contains the authenticator's name.
ms.assetid: f29f5633-e832-4ba3-a3fd-80f557386fec
keywords:
- Name property Virtual Server
- Name property Virtual Server , IVMRCAuthenticator interface
- IVMRCAuthenticator interface Virtual Server , Name property
- Name property Virtual Server , VMRCAuthenticator interface
- VMRCAuthenticator interface Virtual Server , Name property
topic_type:
- apiref
api_name:
- IVMRCAuthenticator.Name
- IVMRCAuthenticator.get_Name
- VMRCAuthenticator.Name
api_location:
- VsComInterfaces.h
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IVMRCAuthenticator::Name property

The **Name** property contains the authenticator's name.

This property is read-only.

## Syntax


```C++
HRESULT get_Name(
  [out] BSTR *name
);
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>VMRCAuthenticator.Name( _
  ByRef name _
)</code></pre></td>
</tr>
</tbody>
</table>



## Property value

The authenticator's name.

This property value is read-only.

## Error codes



| Name                                                                                           | Meaning                                                   |
|------------------------------------------------------------------------------------------------|-----------------------------------------------------------|
| <dl> <dt> S\_OK</dt> </dl>              | The property value was retrieved successfully.<br/> |
| <dl> <dt>E\_POINTER</dt> </dl>          | The *name* parameter is **NULL**.<br/>              |
| <dl> <dt> DISP\_E\_EXCEPTION</dt> </dl> | An unknown error has occurred.<br/>                 |



## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server 2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server 2008orWindows Server 2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMRCAuthenticator**](ivmrcauthenticator.md)
</dt> </dl>

 

 




