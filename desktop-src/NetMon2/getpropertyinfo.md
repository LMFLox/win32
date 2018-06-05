---
Description: The GetPropertyInfo function returns a pointer to the property information of a given protocol.
ms.assetid: f65166ba-1d94-4d65-b9d7-edb84ada0826
title: GetPropertyInfo function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# GetPropertyInfo function

The **GetPropertyInfo** function returns a pointer to the property information of a given protocol.

## Syntax


```C++
LPPROPERTYINFO WINAPI GetPropertyInfo(
  _In_ HPROPERTY hProperty
);
```



## Parameters

<dl> <dt>

*hProperty* \[in\]
</dt> <dd>

Handle to a property.

</dd> </dl>

## Return value

If the function is successful, the return value is a pointer to the property.

If the function is unsuccessful, the return value is **NULL**.

## Remarks

[*Experts*](https://www.bing.com/search?q=*Experts*) and [*parsers*](https://www.bing.com/search?q=*parsers*) can call the **GetPropertyInfo** function.

## Requirements



|                                     |                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                           |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                 |
| Header<br/>                   | <dl> <dt>Netmon.h</dt> </dl>  |
| Library<br/>                  | <dl> <dt>Nmapi.lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl> |



 

 



