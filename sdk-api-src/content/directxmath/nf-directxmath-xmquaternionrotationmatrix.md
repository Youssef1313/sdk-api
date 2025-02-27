---
UID: NF:directxmath.XMQuaternionRotationMatrix
title: XMQuaternionRotationMatrix function (directxmath.h)
description: Computes a rotation quaternion from a rotation matrix.
old-location: dxmath\xmquaternionrotationmatrix.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.quaternion.XMQuaternionRotationMatrix(XMMATRIX)
ms.date: 12/05/2018
ms.keywords: Use DirectX..XMQuaternionRotationMatrix, XMQuaternionRotationMatrix, XMQuaternionRotationMatrix method [DirectX Math Support APIs], dxmath.xmquaternionrotationmatrix
ms.topic: function
f1_keywords:
- directxmath/XMQuaternionRotationMatrix
dev_langs:
- c++
req.header: directxmath.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: Use DirectX.
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- DirectXMath.h
api_name:
- XMQuaternionRotationMatrix
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# XMQuaternionRotationMatrix function


## -description


Computes a rotation quaternion from a rotation matrix.


## -parameters




### -param M [in]

Rotation matrix.


## -returns



Returns the rotation quaternion.




## -remarks



This function only uses the upper 3x3 portion of the <a href="https://docs.microsoft.com/windows/desktop/api/directxmath/ns-directxmath-xmmatrix">XMMATRIX</a>. Note if the input matrix contains scales, shears, or 
    other non-rotation transformations in the upper 3x3 matrix, then the output of this function is ill-defined.

The DirectXMath quaternion functions use an XMVECTOR 4-vector to represent quaternions, 
    where the X, Y, and Z components are the vector part and the W component is the scalar part.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/dxmath/ovw-xnamath-reference-functions-quaternion">DirectXMath Library Quaternion Functions</a>
 

 

