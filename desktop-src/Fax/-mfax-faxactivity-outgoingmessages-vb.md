﻿---
Description: 'The OutgoingMessages property is a number that represents the total number of outgoing fax jobs that the fax service is in the process of sending.'
ms.assetid: '3155080c-d891-4ff5-8fae-d77ee86a2277'
title: 'FaxActivity.OutgoingMessages property'
---

# FaxActivity.OutgoingMessages property

The **OutgoingMessages** property is a number that represents the total number of outgoing fax jobs that the fax service is in the process of sending.

This property is read-only.

## Syntax


```VB
Property OutgoingMessages As Long
```



## Property value

A **Long** that receives the total number of outgoing fax jobs that the fax service is currently sending.

## Remarks

To read this property, a user must have the [****farQUERY\_CONFIG****](-mfax-fax-access-rights-enum.md) access right.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                             |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                    |
| Header<br/>                   | <dl> <dt>FaxComex.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Fxscomex.dll</dt> </dl> |



## See also

<dl> <dt>

[Visual Basic Example](-mfax-monitoring-fax-activity.md)
</dt> <dt>

[**FaxActivity**](-mfax-faxactivity.md)
</dt> <dt>

[**IFaxActivity**](-mfax-faxactivity-cpp.md)
</dt> </dl>

 

 



