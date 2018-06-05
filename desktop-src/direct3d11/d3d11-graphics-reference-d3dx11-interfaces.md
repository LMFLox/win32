---
title: D3DX Interfaces
description: This section contains reference information for the component object model (COM) interfaces provided by the D3DX utility library.
ms.assetid: 0d3be1e6-b558-4586-9440-251a5611d7cd
keywords:
- D3DX interfaces, Direct3D 11
- interfaces, Direct3D 11 D3DX
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# D3DX Interfaces

This section contains reference information for the component object model (COM) interfaces provided by the D3DX utility library.

> [!Note]  
> The D3DX (D3DX 9, D3DX 10, and D3DX 11) utility library is deprecated for Windows 8 and is not supported for Windows Store apps.

 

## 

## In this section



<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Topic</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>[<strong>ID3DX11DataLoader</strong>](id3dx11dataloader.md)<br/></td>
<td><blockquote>
[!Note]<br />
The D3DX (D3DX 9, D3DX 10, and D3DX 11) utility library is deprecated for Windows 8 and is not supported for Windows Store apps.
</blockquote>
<br/> Data loading object used by [<strong>ID3DX11ThreadPump Interface</strong>](id3dx11threadpump.md) for loading data asynchronously.<br/></td>
</tr>
<tr class="even">
<td>[<strong>ID3DX11DataProcessor</strong>](id3dx11dataprocessor.md)<br/></td>
<td><blockquote>
[!Note]<br />
The D3DX (D3DX 9, D3DX 10, and D3DX 11) utility library is deprecated for Windows 8 and is not supported for Windows Store apps.
</blockquote>
<br/> Data processing object used by [<strong>ID3DX11ThreadPump Interface</strong>](id3dx11threadpump.md) for loading data asynchronously.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>ID3DX11ThreadPump</strong>](id3dx11threadpump.md)<br/></td>
<td><blockquote>
[!Note]<br />
The D3DX (D3DX 9, D3DX 10, and D3DX 11) utility library is deprecated for Windows 8 and is not supported for Windows Store apps.
</blockquote>
<br/> A thread pump executes tasks asynchronously. It is created by calling [<strong>D3DX11CreateThreadPump</strong>](d3dx11createthreadpump.md). There are several APIs that take an optional thread pump as a parameter, such as [<strong>D3DX11CreateTextureFromFile</strong>](d3dx11createtexturefromfile.md) and [<strong>D3DX11CompileFromFile</strong>](d3dx11compilefromfile.md); if you pass a thread pump interface into these APIs, the functions will execute asynchronously on a separate thread. Particularly on multiprocessor machines, a thread pump can load resources and process data without a noticeable decrease in performance.<br/></td>
</tr>
</tbody>
</table>



 

## Related topics

<dl> <dt>

[D3DX 11 Reference](d3d11-graphics-reference-d3dx11.md)
</dt> </dl>

 

 




