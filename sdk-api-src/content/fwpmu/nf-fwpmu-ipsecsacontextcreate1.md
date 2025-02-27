---
UID: NF:fwpmu.IPsecSaContextCreate1
title: IPsecSaContextCreate1 function (fwpmu.h)
description: Creates an IPsec security association (SA) context.
old-location: fwp\ipsecsacontextcreate1.htm
tech.root: fwp
ms.assetid: b0eab185-fae2-4133-b3f2-22d609cb94d1
ms.date: 12/05/2018
ms.keywords: IPsecSaContextCreate1, IPsecSaContextCreate1 function [Filtering], fwp.ipsecsacontextcreate1, fwpmu/IPsecSaContextCreate1
ms.topic: function
f1_keywords:
- fwpmu/IPsecSaContextCreate1
dev_langs:
- c++
req.header: fwpmu.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Fwpuclnt.lib
req.dll: Fwpuclnt.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Fwpuclnt.dll
api_name:
- IPsecSaContextCreate1
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPsecSaContextCreate1 function


## -description


The <b>IPsecSaContextCreate1</b> function creates an IPsec security association (SA) context.
<div class="alert"><b>Note</b>  <b>IPsecSaContextCreate1</b> is the specific implementation of IPsecSaContextCreate used in Windows 7 and later. See <a href="https://docs.microsoft.com/windows/desktop/FWP/wfp-version-independent-names-and-targeting-specific-versions-of-windows">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows Vista, <a href="https://docs.microsoft.com/windows/desktop/api/fwpmu/nf-fwpmu-ipsecsacontextcreate0">IPsecSaContextCreate0</a> is available.</div><div> </div>

## -parameters




### -param engineHandle [in]

Type: <b>HANDLE</b>

Handle for an open session to the filter engine. Call <a href="https://docs.microsoft.com/windows/desktop/api/fwpmu/nf-fwpmu-fwpmengineopen0">FwpmEngineOpen0</a> to open a session to the filter engine.


### -param outboundTraffic [in]

Type: [IPSEC_TRAFFIC1](https://docs.microsoft.com/windows/desktop/api/ipsectypes/ns-ipsectypes-ipsec_traffic0)a>*</b>

The outbound traffic of the SA.


### -param virtualIfTunnelInfo [in, optional]

Type: [IPSEC_VIRTUAL_IF_TUNNEL_INFO0](https://docs.microsoft.com/windows/desktop/api/fwptypes/ns-fwptypes-ipsec_virtual_if_tunnel_info0)a>*</b>

Details related to virtual interface tunneling.


### -param inboundFilterId [out, optional]

Type: <b>UINT64*</b>

 Optional filter identifier of the cached inbound filter corresponding to the <i>outboundTraffic</i> parameter specified by the caller. Base filtering engine (BFE) may cache the inbound filter identifier and return the cached value, if available. Caller must handle the case when BFE does not have a cached value, in which case this parameter will be set to 0.


### -param id [out]

Type: <b>UINT64*</b>

The identifier of the  IPsec SA context.


## -returns



Type: <b>DWORD</b>

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The IPsec SA context was created successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>FWP_E_* error code</b></dt>
<dt>0x80320001—0x80320039</dt>
</dl>
</td>
<td width="60%">
A Windows Filtering Platform (WFP) specific error. See <a href="https://docs.microsoft.com/windows/desktop/FWP/wfp-error-codes">WFP Error Codes</a> for details.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_* error code</b></dt>
<dt>0x80010001—0x80010122</dt>
</dl>
</td>
<td width="60%">
Failure to communicate with the remote or local firewall engine.

</td>
</tr>
</table>
 




## -remarks



This function cannot be called from within a transaction. It will fail with
<b>FWP_E_TXN_IN_PROGRESS</b>. See <a href="https://docs.microsoft.com/windows/desktop/FWP/object-management">Object Management</a> for more information about transactions.

This function cannot be called from within a dynamic session. The call will fail with <b>FWP_E_DYNAMIC_SESSION_IN_PROGRESS</b>. See <a href="https://docs.microsoft.com/windows/desktop/FWP/object-management">Object Management</a> for more information about dynamic sessions.

The caller needs <a href="https://docs.microsoft.com/windows/desktop/FWP/access-right-identifiers">FWPM_ACTRL_ADD</a> access to the IPsec security associations database. See <a href="https://docs.microsoft.com/windows/desktop/FWP/access-control">Access Control</a> for more information.




## -see-also




[IPSEC_TRAFFIC1](https://docs.microsoft.com/windows/desktop/api/ipsectypes/ns-ipsectypes-ipsec_traffic0)a>



[IPSEC_VIRTUAL_IF_TUNNEL_INFO0](https://docs.microsoft.com/windows/desktop/api/fwptypes/ns-fwptypes-ipsec_virtual_if_tunnel_info0)a>
 

 

