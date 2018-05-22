---
title: D3D12GetFormatPlaneCount function
description: Gets the number of planes for the specified DXGI format for the specified virtual adapter (an ID3D12Device).
ms.assetid: 'CD21F6F9-A9AA-4CE8-A430-57C70326CB4B'
keywords: ["D3D12GetFormatPlaneCount function"]
topic_type:
- apiref
api_name:
- D3D12GetFormatPlaneCount
api_location:
- D3D12.dll
api_type:
- DllExport
---

# D3D12GetFormatPlaneCount function

Gets the number of planes for the specified DXGI format for the specified virtual adapter (an **ID3D12Device**).

## Syntax


```C++
UINT8 inline D3D12GetFormatPlaneCount(
  _In_�ID3D12Device *pDevice,
  �����DXGI_FORMAT �Format
);
```



## Parameters

<dl> <dt>

*pDevice* \[in\]
</dt> <dd>

Type: **[**ID3D12Device**](id3d12device.md)\***

The virtual adapter (an [**ID3D12Device**](id3d12device.md)) for which to get the plane count.

</dd> <dt>

*Format* 
</dt> <dd>

Type: **[**DXGI\_FORMAT**](https://msdn.microsoft.com/library/windows/desktop/bb173059)**

The [**DXGI\_FORMAT**](https://msdn.microsoft.com/library/windows/desktop/bb173059) for which to get the plane count.

</dd> </dl>

## Return value

Type: **UINT8**

The plane count for the specified format on the specified virtual adapter.

## Requirements



|                    |                                                                                      |
|--------------------|--------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx12.h</dt> </dl>  |
| Library<br/> | <dl> <dt>D3D12.lib</dt> </dl> |
| DLL<br/>     | <dl> <dt>D3D12.dll</dt> </dl> |



## See also

<dl> <dt>

[**D3D12\_FEATURE\_DATA\_FORMAT\_INFO**](d3d12-feature-data-format-info.md)
</dt> <dt>

[**CheckFeatureSupport**](id3d12device-checkfeaturesupport.md)
</dt> <dt>

[Helper Functions for D3D12](helper-functions-for-d3d12.md)
</dt> </dl>

�

�




