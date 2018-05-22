---
Description: 'Flag indicating whether the release callback is enabled. This flag is set in the constructor method. If the value is FALSE, calling the CBaseAllocator::SetNotify method causes an assertion to fire (in debug builds).'
ms.assetid: 'cc9adc7c-ec44-41e7-875a-b3e553120804'
title: 'CBaseAllocator::m\_fEnableReleaseCallback member'
---

# CBaseAllocator::m\_fEnableReleaseCallback member

Flag indicating whether the release callback is enabled. This flag is set in the constructor method. If the value is **FALSE**, calling the [**CBaseAllocator::SetNotify**](cbaseallocator-setnotify.md) method causes an assertion to fire (in debug builds).

## Syntax


```C++
BOOL m_fEnableReleaseCallback;
```



## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Amfilter.h (include Streams.h)</dt> </dl>                                                                                  |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CBaseAllocator Class**](cbaseallocator.md)
</dt> </dl>

�

�



