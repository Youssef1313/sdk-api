---
UID: NF:clusapi.ClusterNetworkControl
title: ClusterNetworkControl function (clusapi.h)
description: Initiates an operation on a network. The operation performed depends on the control code passed to the dwControlCode parameter.
old-location: mscs\clusternetworkcontrol.htm
tech.root: MsCS
ms.assetid: df0d7b45-4d8b-4780-944a-0fbba670f99a
ms.date: 12/05/2018
ms.keywords: ClusterNetworkControl, ClusterNetworkControl function [Failover Cluster], _wolf_clusternetworkcontrol, clusapi/ClusterNetworkControl, mscs.clusternetworkcontrol
ms.topic: function
f1_keywords:
- clusapi/ClusterNetworkControl
dev_langs:
- c++
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Enterprise, Windows Server 2008 Datacenter
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: ClusAPI.lib
req.dll: ClusAPI.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- ClusAPI.dll
api_name:
- ClusterNetworkControl
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ClusterNetworkControl function


## -description


Initiates 
    an operation on a <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/networks">network</a>. The operation performed depends on the 
    <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/control-codes">control code</a> passed to the 
    <i>dwControlCode</i> parameter.


## -parameters




### -param hNetwork [in]

Handle to the network to be affected by the operation.


### -param hHostNode [in, optional]

If non-<b>NULL</b>, handle to the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/nodes">node</a> 
       hosting the affected network. If <b>NULL</b>, the local node performs the operation. 
       Specifying <i>hHostNode</i> is optional.


### -param dwControlCode [in]

A <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/network-control-codes">network control code</a> specifying the 
       operation to be performed. For the syntax associated with a control code, refer to  
       <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/control-code-architecture">Control Code Architecture</a> and the following 
       topics:


<ul>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-enum-common-properties">CLUSCTL_NETWORK_ENUM_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-enum-private-properties">CLUSCTL_NETWORK_ENUM_PRIVATE_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-characteristics">CLUSCTL_NETWORK_GET_CHARACTERISTICS</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-common-properties">CLUSCTL_NETWORK_GET_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-common-property-fmts">CLUSCTL_NETWORK_GET_COMMON_PROPERTY_FMTS</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-flags">CLUSCTL_NETWORK_GET_FLAGS</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-id">CLUSCTL_NETWORK_GET_ID</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-name">CLUSCTL_NETWORK_GET_NAME</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-private-properties">CLUSCTL_NETWORK_GET_PRIVATE_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-private-property-fmts">CLUSCTL_NETWORK_GET_PRIVATE_PROPERTY_FMTS</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-ro-common-properties">CLUSCTL_NETWORK_GET_RO_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-get-ro-private-properties">CLUSCTL_NETWORK_GET_RO_PRIVATE_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-set-common-properties">CLUSCTL_NETWORK_SET_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-set-private-properties">CLUSCTL_NETWORK_SET_PRIVATE_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-unknown">CLUSCTL_NETWORK_UNKNOWN</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-validate-common-properties">CLUSCTL_NETWORK_VALIDATE_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/clusctl-network-validate-private-properties">CLUSCTL_NETWORK_VALIDATE_PRIVATE_PROPERTIES</a>
</li>
</ul>



### -param lpInBuffer [in, optional]

Pointer to an input buffer containing information needed for the operation, or <b>NULL</b> 
       if no information is needed.


### -param nInBufferSize [in]

The allocated size (in bytes) of the input buffer.


### -param lpOutBuffer [out, optional]

Pointer to an output buffer to receive the data resulting from the operation, or 
       <b>NULL</b> if no data will be returned.


### -param nOutBufferSize [in]

The allocated size (in bytes) of the output buffer.


### -param lpBytesReturned [in, out, optional]

Returns the actual size (in bytes) of the data resulting from the operation. If this information is not 
       needed, pass <b>NULL</b> for <i>lpBytesReturned</i>.


## -returns



The function returns one of the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
</dl>
</td>
<td width="60%">
The operation was successful. If the operation required an output buffer, 
         <i>lpBytesReturned</i> (if not <b>NULL</b> on input) points to the 
         actual size of the data returned in the buffer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_MORE_DATA</b></dt>
</dl>
</td>
<td width="60%">
The output buffer pointed to by <i>lpOutBuffer</i> was not large enough to hold the data 
         resulting from the operation. The <i>lpBytesReturned</i> parameter (if not 
         <b>NULL</b> on input) points to the size required for the output buffer. Only operations 
         requiring an output buffer return <b>ERROR_MORE_DATA</b>. If the 
         <i>lpOutBuffer</i> parameter is <b>NULL</b> and the 
         <i>nOutBufferSize</i> parameter is zero, then <b>ERROR_SUCCESS</b> may 
         be returned, not <b>ERROR_MORE_DATA</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://docs.microsoft.com/windows/desktop/Debug/system-error-codes">System error code</a></b></dt>
</dl>
</td>
<td width="60%">
The operation was not successful. If the operation required an output buffer, the value specified by 
         <i>lpBytesReturned</i> (if not <b>NULL</b> on input) is unreliable.

</td>
</tr>
</table>
 




## -remarks



If <b>ClusterNetworkControl</b> returns 
     <b>ERROR_MORE_DATA</b>, set <i>nOutBufferSize</i> to the number of bytes 
     pointed to by <i>lpBytesReturned</i>, and call the function again.

Do not pass LPC and RPC handles to the same function call. Otherwise, the call will raise an RPC exception and 
     can have additional destructive effects. For information on how LPC and RPC handles are created, see 
     <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/lpc-and-rpc-handles">LPC and RPC Handles</a> and 
     <a href="https://docs.microsoft.com/windows/desktop/api/clusapi/nf-clusapi-opencluster">OpenCluster</a>.

<b>ClusterNetworkControl</b> is one of the 
     <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/control-code-functions">control code functions</a>. For more information on 
     control codes and control code functions, see 
     <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/using-control-codes">Using Control Codes</a>.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/network-control-codes">Network Control Codes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/clusapi/nf-clusapi-opencluster">OpenCluster</a>
 

 

