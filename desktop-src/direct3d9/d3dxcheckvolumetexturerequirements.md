﻿---
Description: 'Checks volume-texture-creation parameters.'
ms.assetid: '1a02cb99-2582-4d8f-aacf-67ed75f6deb8'
title: D3DXCheckVolumeTextureRequirements function
---

# D3DXCheckVolumeTextureRequirements function

Checks volume-texture-creation parameters.

## Syntax


```C++
HRESULT D3DXCheckVolumeTextureRequirements(
  _In_    LPDIRECT3DDEVICE9 pDevice,
  _Inout_ UINT              *pWidth,
  _Inout_ UINT              *pHeight,
  _Inout_ UINT              *pDepth,
  _Inout_ UINT              *pNumMipLevels,
  _In_    DWORD             Usage,
  _Inout_ D3DFORMAT         *pFormat,
  _In_    D3DPOOL           Pool
);
```



## Parameters

<dl> <dt>

*pDevice* \[in\]
</dt> <dd>

Type: **[**LPDIRECT3DDEVICE9**](idirect3ddevice9.md)**

Pointer to an [**IDirect3DDevice9**](idirect3ddevice9.md) interface, representing the device to be associated with the volume texture.

</dd> <dt>

*pWidth* \[in, out\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)\***

Pointer to the requested width in pixels, or **NULL**. Returns the corrected size.

</dd> <dt>

*pHeight* \[in, out\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)\***

Pointer to the requested height in pixels, or **NULL**. Returns the corrected size.

</dd> <dt>

*pDepth* \[in, out\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)\***

Pointer to the requested depth in pixels, or **NULL**. Returns the corrected size.

</dd> <dt>

*pNumMipLevels* \[in, out\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)\***

Pointer to the number of requested mipmap levels, or **NULL**. Returns the corrected number of mipmap levels.

</dd> <dt>

*Usage* \[in\]
</dt> <dd>

Type: **[**DWORD**](winprog.windows_data_types)**

Currently not used, set to 0.

</dd> <dt>

*pFormat* \[in, out\]
</dt> <dd>

Type: **[D3DFORMAT](d3dformat.md)\***

Pointer to a member of the [D3DFORMAT](d3dformat.md) enumerated type. Specifies the desired pixel format, or **NULL**. Returns the corrected format.

</dd> <dt>

*Pool* \[in\]
</dt> <dd>

Type: **[**D3DPOOL**](direct3d9.d3dpool)**

Member of the [**D3DPOOL**](direct3d9.d3dpool) enumerated type, describing the memory class into which the volume texture should be placed.

</dd> </dl>

## Return value

Type: **[**HRESULT**](455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the function succeeds, the return value is D3D\_OK. If the function fails, the return value can be one of the following: D3DERR\_NOTAVAILABLE, D3DERR\_INVALIDCALL.

## Remarks

If parameters to this function are invalid, this function returns corrected parameters.

## Requirements



|                    |                                                                                       |
|--------------------|---------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx9tex.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>  |



## See also

<dl> <dt>

[Texture Functions in D3DX 9](dx9-graphics-reference-d3dx-functions-texture.md)
</dt> </dl>

 

 



