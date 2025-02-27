---
UID: NF:directxpackedvector.XMXDECN4.XMXDECN4(uint32_t)
title: XMXDECN4::XMXDECN4(uint32_t) (directxpackedvector.h)
description: Initializes a new instance of XMXDECN4 from a uint32_t variable containing component data in a packed format.
old-location: dxmath\xmxdecn4_ctor_2.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMXDECN4.#ctor(uint32_t)
ms.date: 12/05/2018
ms.keywords: XMXDECN4, XMXDECN4 constructor [DirectX Math Support APIs], XMXDECN4 constructor [DirectX Math Support APIs],XMXDECN4 structure, XMXDECN4 structure [DirectX Math Support APIs],XMXDECN4 constructor, XMXDECN4.XMXDECN4, XMXDECN4.XMXDECN4(uint32_t), XMXDECN4::XMXDECN4, XMXDECN4::XMXDECN4(uint32_t), dxmath.xmxdecn4_ctor_2
ms.topic: method
f1_keywords:
- directxpackedvector/XMXDECN4.XMXDECN4
dev_langs:
- c++
req.header: directxpackedvector.h
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
req.namespace: DirectX::PackedVector
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
- DirectXPackedVector.h
api_name:
- XMXDECN4.XMXDECN4
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# XMXDECN4::XMXDECN4(uint32_t)


## -description


Initializes a new instance of <code>XMXDECN4</code> from a <code>uint32_t</code> variable containing
	component data in a packed format.
    

This constructor initializes a new instance of <a href="https://docs.microsoft.com/windows/desktop/api/directxpackedvector/ns-directxpackedvector-xmxdecn4">XMXDECN4 </a> from a
	<code>uint32_t</code> variable containing component data in a packed format.
<div class="alert"><b>Note</b>  This constructor is only available under C++.
    </div><div> </div>

## -parameters




### -param Packed

The values of four vector components in a packed format.
		    
		


## -remarks



The values defining the four components of the new instance of <code>XMXDECN4</code> are
	    not normalized and are stored in the argument <code>Packed</code> as follows:
	

<ul>
<li>
The first 10 bits (bits 0-9) of <b>Packed</b> assigned, as a signed
		    integer, to the <b>x</b> member of the instance of <code>XMXDECN4</code>constructed.
		

</li>
<li>
The second 10 bits (bits 10-19) of <b>Packed</b> assigned, as a signed
		    integer, to the <b>y</b> member of the instance of <code>XMXDECN4</code>constructed.
		

</li>
<li>
The third 10 bits (bits 20-29) of <b>Packed</b> assigned, as a signed
		    integer, to the <b>z</b> member of the instance of <code>XMXDECN4</code>constructed.
		

</li>
<li>
The last 2 bits (bits 30-31) of <b>Packed</b> assigned, as an unsigned
		    integer, to the <b>w</b> member of the instance of <code>XMXDECN4</code>constructed.
		

</li>
</ul>



## -see-also




<b>Reference</b>



<a href="https://docs.microsoft.com/windows/desktop/api/directxpackedvector/ns-directxpackedvector-xmxdecn4">XMXDECN4</a>



<a href="https://docs.microsoft.com/windows/desktop/dxmath/xmxdecn4-ctor">XMXDECN4 Constructors</a>
 

 

