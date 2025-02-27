---
UID: NS:ntdsapi._DS_REPL_KCC_DSA_FAILURESW
title: DS_REPL_KCC_DSA_FAILURESW (ntdsapi.h)
description: The DS_REPL_KCC_DSA_FAILURES structure contains an array of DS_REPL_KCC_DSA_FAILURE structures, which in turn contain replication state data with respect to inbound replication partners, as returned by the DsReplicaGetInfo and DsReplicaGetInfo2 functions.
old-location: ad\ds_repl_kcc_dsa_failures.htm
tech.root: ad
ms.assetid: bb011502-38ae-43b7-a6ad-de16b499f61b
ms.date: 12/05/2018
ms.keywords: DS_REPL_KCC_DSA_FAILURES, DS_REPL_KCC_DSA_FAILURES structure [Active Directory], DS_REPL_KCC_DSA_FAILURESW, _glines_ds_repl_kcc_dsa_failures, ad.ds__repl__kcc__dsa__failures, ad.ds_repl_kcc_dsa_failures, ntdsapi/DS_REPL_KCC_DSA_FAILURES
ms.topic: struct
f1_keywords:
- ntdsapi/DS_REPL_KCC_DSA_FAILURES
dev_langs:
- c++
req.header: ntdsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
- Ntdsapi.h
api_name:
- DS_REPL_KCC_DSA_FAILURES
targetos: Windows
req.typenames: DS_REPL_KCC_DSA_FAILURESW
req.redist: 
ms.custom: 19H1
---

# DS_REPL_KCC_DSA_FAILURESW structure


## -description


The <b>DS_REPL_KCC_DSA_FAILURES</b> structure contains an array of <a href="https://docs.microsoft.com/windows/desktop/api/ntdsapi/ns-ntdsapi-ds_repl_kcc_dsa_failurew">DS_REPL_KCC_DSA_FAILURE</a> structures, which in turn contain replication state data with respect to inbound replication partners, as returned by the 
<a href="https://docs.microsoft.com/windows/desktop/api/ntdsapi/nf-ntdsapi-dsreplicagetinfow">DsReplicaGetInfo</a> and <a href="https://docs.microsoft.com/windows/desktop/api/ntdsapi/nf-ntdsapi-dsreplicagetinfo2w">DsReplicaGetInfo2</a> functions.


## -struct-fields




### -field cNumEntries

Contains the number of elements in the <b>rgMetaData</b> array.


### -field dwReserved

Reserved for future use.


### -field rgDsaFailure.size_is

 


### -field rgDsaFailure.size_is.cNumEntries

 


### -field rgDsaFailure

Contains an array of <a href="https://docs.microsoft.com/windows/desktop/api/ntdsapi/ns-ntdsapi-ds_repl_kcc_dsa_failurew">DS_REPL_KCC_DSA_FAILURE</a> structures that contain the requested replication data. The <b>cNumEntries</b> member contains the number of elements in this array.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/ntdsapi/ns-ntdsapi-ds_repl_kcc_dsa_failurew">DS_REPL_KCC_DSA_FAILURE</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ntdsapi/nf-ntdsapi-dsreplicagetinfow">DsReplicaGetInfo</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ntdsapi/nf-ntdsapi-dsreplicagetinfo2w">DsReplicaGetInfo2</a>
 

 

