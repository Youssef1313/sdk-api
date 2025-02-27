---
UID: NF:p2p.PeerGroupShutdown
title: PeerGroupShutdown function (p2p.h)
description: The PeerGroupShutdown function closes a peer group created with PeerGroupStartup and disposes of any allocated resources.
old-location: p2p\peergroupshutdown.htm
tech.root: P2PSdk
ms.assetid: 61678a50-71cd-4717-b490-2755c605c2d5
ms.date: 12/05/2018
ms.keywords: PeerGroupShutdown, PeerGroupShutdown function [Peer Networking], p2p.peergroupshutdown, p2p/PeerGroupShutdown
ms.topic: function
f1_keywords:
- p2p/PeerGroupShutdown
dev_langs:
- c++
req.header: p2p.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only],Windows XP with SP1 with the Advanced Networking Pack forWindows XP
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: P2P.lib
req.dll: P2P.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- P2P.dll
api_name:
- PeerGroupShutdown
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# PeerGroupShutdown function


## -description


The <b>PeerGroupShutdown</b> function closes a peer group created with <a href="https://docs.microsoft.com/windows/desktop/api/p2p/nf-p2p-peergroupstartup">PeerGroupStartup</a> and disposes of any allocated resources.


## -parameters






## -returns



Returns <b>S_OK</b> if the operation succeeds. Otherwise, the function returns  the following value.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
The function terminated unexpectedly.

</td>
</tr>
</table>
 

Cryptography-specific errors can be returned from the <a href="https://docs.microsoft.com/windows/desktop/SecCrypto/microsoft-base-cryptographic-provider">Microsoft RSA Base Provider</a>. These errors are prefixed with CRYPT_* and defined in Winerror.h.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/P2PSdk/grouping-api-functions">Grouping API
		  Functions</a>



<a href="https://docs.microsoft.com/windows/desktop/api/p2p/nf-p2p-peergroupstartup">PeerGroupStartup</a>
 

 

