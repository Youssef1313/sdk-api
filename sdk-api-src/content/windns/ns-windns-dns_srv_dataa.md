---
UID: NS:windns.__unnamed_struct_31
title: DNS_SRV_DATAA (windns.h)
description: The DNS_SRV_DATA structure represents a DNS service (SRV) record as specified in RFC 2782.
old-location: dns\dns_srv_data.htm
tech.root: DNS
ms.assetid: 212db7ac-a5e3-4e58-b1c2-0eb551403dfc
ms.date: 12/05/2018
ms.keywords: '*PDNS_SRV_DATA, *PDNS_SRV_DATAA, DNS_SRV_DATA, DNS_SRV_DATA structure [DNS], DNS_SRV_DATAA, PDNS_SRV_DATA, PDNS_SRV_DATA structure pointer [DNS], _dns_dns_srv_data, dns.dns_srv_data, windns/DNS_SRV_DATA, windns/PDNS_SRV_DATA'
ms.topic: struct
f1_keywords:
- windns/DNS_SRV_DATA
dev_langs:
- c++
req.header: windns.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
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
- Windns.h
api_name:
- DNS_SRV_DATA
targetos: Windows
req.typenames: DNS_SRV_DATAA, *PDNS_SRV_DATAA
req.redist: 
ms.custom: 19H1
---

# DNS_SRV_DATAA structure


## -description


The 
<b>DNS_SRV_DATA</b> structure represents a DNS service (SRV) record as specified in <a href="http://go.microsoft.com/fwlink/p/?linkid=90381">RFC 2782</a>.


## -struct-fields




### -field pNameTarget

A pointer to a string that represents the target host.


### -field wPriority

The priority of the target host specified in <b>pNameTarget</b>. Lower numbers imply higher priority to clients attempting to use this service.


### -field wWeight

The relative weight of the target host in <b>pNameTarget</b> to other hosts with the same <b>wPriority</b>. The chances of using this host should be proportional to its weight.


### -field wPort

The port used on the target host for this service.


### -field Pad

Reserved for padding. Do not use.


## -remarks



The 
<b>DNS_SRV_DATA</b> structure is used in conjunction with the 
<a href="https://docs.microsoft.com/windows/win32/api/windns/ns-windns-dns_recorda">DNS_RECORD</a> structure to programmatically manage DNS entries.




## -see-also




<a href="https://docs.microsoft.com/windows/win32/api/windns/ns-windns-dns_recorda">DNS_RECORD</a>
 

 

