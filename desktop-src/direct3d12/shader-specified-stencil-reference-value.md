---
title: Shader Specified Stencil Reference Value
description: Enabling pixel shaders to output the Stencil Reference Value, rather than using the API-specified one, enables a very fine granular control over stencil operations.
ms.assetid: 'F58B1930-F12E-4FA4-A15C-A3C2B8705033'
---

# Shader Specified Stencil Reference Value

Enabling pixel shaders to output the Stencil Reference Value, rather than using the API-specified one, enables a very fine granular control over stencil operations.

The Stencil Reference Value is normally specified by the [**ID3D12GraphicsCommandList::OMSetStencilRef**](id3d12graphicscommandlist-omsetstencilref.md) method. This method sets the stencil reference value on a per-draw granularity. However, this value can be overwritten by the pixel shader.

This D3D12 (and D3D11.3) feature enables developers to read and use the Stencil Reference Value (*SV\_StencilRef*) that is output from a pixel shader, enabling a per-pixel or per-sample granularity.

The shader specified value replaces the API-specified reference value for that invocation, which means the change affects both the stencil test, and when the stencil operation D3D12\_STENCIL\_OP\_REPLACE (one member of [**D3D12\_STENCIL\_OP**](d3d12-stencil-op.md)) is used to write the reference value to the stencil buffer.

This feature is optional in both D3D12 and D3D11.3. To test for its support, check the *PSSpecifiedStencilRefSupported* boolean field of [**D3D12\_FEATURE\_DATA\_D3D12\_OPTIONS**](d3d12-feature-data-d3d12-options.md) using [**CheckFeatureSupport**](id3d12device-checkfeaturesupport.md).

Here is an example of the use of *SV\_StencilRef* in a pixel shader:

``` syntax
float main2(float4 c : COORD) : SV_StencilRef
{
    return c;
}
```

## Related topics

<dl> <dt>

[Rendering](rendering.md)
</dt> <dt>

[Resource Binding in HLSL](resource-binding-in-hlsl.md)
</dt> <dt>

[Shader Model 5.1](https://msdn.microsoft.com/library/windows/desktop/dn933277)
</dt> <dt>

[Specifying Root Signatures in HLSL](specifying-root-signatures-in-hlsl.md)
</dt> </dl>

 

 



