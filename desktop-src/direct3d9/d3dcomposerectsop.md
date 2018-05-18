﻿---
Description: 'Specifies how to combine the glyph data from the source and destination surfaces in a call to ComposeRects.'
ms.assetid: '4b0e6e48-48e0-4955-bb20-f953fdce785c'
title: D3DCOMPOSERECTSOP enumeration
---

# D3DCOMPOSERECTSOP enumeration

Specifies how to combine the glyph data from the source and destination surfaces in a call to [**ComposeRects**](idirect3ddevice9ex-composerect.md).

## Syntax


```C++
typedef enum _D3DCOMPOSERECTSOP { 
  D3DCOMPOSERECTS_COPY         = 1,
  D3DCOMPOSERECTS_OR           = 2,
  D3DCOMPOSERECTS_AND          = 3,
  D3DCOMPOSERECTS_NEG          = 4,
  D3DCOMPOSERECTS_FORCE_DWORD  = 0x7fffffff
} D3DCOMPOSERECTSOP;
```



## Constants

<dl> <dt>

<span id="D3DCOMPOSERECTS_COPY"></span><span id="d3dcomposerects_copy"></span>**D3DCOMPOSERECTS\_COPY**
</dt> <dd>

Copy the source to the destination.

</dd> <dt>

<span id="D3DCOMPOSERECTS_OR"></span><span id="d3dcomposerects_or"></span>**D3DCOMPOSERECTS\_OR**
</dt> <dd>

Bitwise OR the source and the destination.

</dd> <dt>

<span id="D3DCOMPOSERECTS_AND"></span><span id="d3dcomposerects_and"></span>**D3DCOMPOSERECTS\_AND**
</dt> <dd>

Bitwise AND the source and the destination.

</dd> <dt>

<span id="D3DCOMPOSERECTS_NEG"></span><span id="d3dcomposerects_neg"></span>**D3DCOMPOSERECTS\_NEG**
</dt> <dd>

Copy the negated source to the destination (Dst & ~Src).

</dd> <dt>

<span id="D3DCOMPOSERECTS_FORCE_DWORD"></span><span id="d3dcomposerects_force_dword"></span>**D3DCOMPOSERECTS\_FORCE\_DWORD**
</dt> <dd>

Reserved. Used to force enumeration to 32-bits in size.

</dd> </dl>

## Requirements



|                   |                                                                                        |
|-------------------|----------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>D3d9types.h</dt> </dl> |



## See also

<dl> <dt>

[Direct3D Enumerations](dx9-graphics-reference-d3d-enums.md)
</dt> </dl>

 

 



