---
UID: NF:rtmv2.RTM_IPV4_GET_ADDR_AND_MASK
title: RTM_IPV4_GET_ADDR_AND_MASK macro (rtmv2.h)
description: The RTM_IPV4_GET_ADDR_AND_MASK macro converts to a generic RTM_NET_ADDRESS structure and length to an IPv4 address and mask.
old-location: rras\rtm_ipv4_get_addr_and_mask.htm
tech.root: RRAS
ms.assetid: 2dd2c01b-41f1-48e3-942b-954f7b2efac5
ms.date: 12/05/2018
ms.keywords: RTM_IPV4_GET_ADDR_AND_MASK, RTM_IPV4_GET_ADDR_AND_MASK macro [RAS], _rtmv2ref_rtm_ipv4_get_addr_and_mask, rras.rtm_ipv4_get_addr_and_mask, rtmv2/RTM_IPV4_GET_ADDR_AND_MASK
ms.topic: macro
f1_keywords:
- rtmv2/RTM_IPV4_GET_ADDR_AND_MASK
dev_langs:
- c++
req.header: rtmv2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- Rtmv2.h
api_name:
- RTM_IPV4_GET_ADDR_AND_MASK
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# RTM_IPV4_GET_ADDR_AND_MASK macro


## -description


The 
<b>RTM_IPV4_GET_ADDR_AND_MASK</b> macro converts to a generic 
<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/ns-rtmv2-rtm_net_address">RTM_NET_ADDRESS</a> structure and length to an IPv4 address and mask.


## -parameters




### -param Addr

Receives the converted IPv4 address.


### -param Mask

Receives the converted IPv4 mask.


### -param NetAddress

Specifies the network address to convert.


## -remarks



For example, if a client supplies the <i>NetAddress</i> 10.10.10.24, the <i>Addr</i> 10.10.10.0 and the <i>Mask</i> 255.255.255.255 are returned.

The macro is defined as follows:


```cpp
#include <windows.h>

#define RTM_IPV4_GET_ADDR_AND_MASK(Addr, Mask, NetAddress)  \
        (Addr) = (* (ULONG *) ((NetAddress)->AddrBits));    \
        (Mask) = RTM_IPV4_MASK_FROM_LEN((NetAddress)-       \
            >NumBits);   

```





## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/nf-rtmv2-rtm_ipv4_get_addr_and_len">RTM_IPV4_GET_ADDR_AND_LEN</a>



<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/nf-rtmv2-rtm_ipv4_len_from_mask">RTM_IPV4_LEN_FROM_MASK</a>



<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/nf-rtmv2-rtm_ipv4_make_net_address">RTM_IPV4_MAKE_NET_ADDRESS</a>



<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/nf-rtmv2-rtm_ipv4_mask_from_len">RTM_IPV4_MASK_FROM_LEN</a>



<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/nf-rtmv2-rtm_ipv4_set_addr_and_len">RTM_IPV4_SET_ADDR_AND_LEN</a>



<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/nf-rtmv2-rtm_ipv4_set_addr_and_mask">RTM_IPV4_SET_ADDR_AND_MASK</a>



<a href="https://docs.microsoft.com/windows/desktop/api/rtmv2/ns-rtmv2-rtm_net_address">RTM_NET_ADDRESS</a>
 

 

