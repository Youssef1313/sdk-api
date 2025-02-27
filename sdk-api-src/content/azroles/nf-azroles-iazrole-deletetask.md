---
UID: NF:azroles.IAzRole.DeleteTask
title: IAzRole::DeleteTask (azroles.h)
description: Removes the IAzTask object with the specified name from the role.
old-location: security\iazrole_deletetask.htm
tech.root: SecAuthZ
ms.assetid: 62623d45-33a6-4e3f-b0a8-d3e3e7c9e33e
ms.date: 12/05/2018
ms.keywords: AzRole object [Security],DeleteTask method, DeleteTask, DeleteTask method [Security], DeleteTask method [Security],AzRole object, DeleteTask method [Security],IAzRole interface, IAzRole interface [Security],DeleteTask method, IAzRole.DeleteTask, IAzRole::DeleteTask, azroles/IAzRole::DeleteTask, security.iazrole_deletetask
ms.topic: method
f1_keywords:
- azroles/IAzRole.DeleteTask
dev_langs:
- c++
req.header: azroles.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Azroles.lib
req.dll: Azroles.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Azroles.dll
api_name:
- IAzRole.DeleteTask
- AzRole.DeleteTask
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
ms.custom: 19H1
---

# IAzRole::DeleteTask


## -description


The <b>DeleteTask</b> method removes the <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iaztask">IAzTask</a> object with the specified name from the role.


## -parameters




### -param bstrProp [in]

Name of the <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iaztask">IAzTask</a> object to remove from the role.


### -param varReserved [in, optional]

Reserved for future use.


## -remarks



If there are any <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iaztask">IAzTask</a> references to an <b>IAzTask</b> object that has been deleted from the cache, the <b>IAzTask</b> object can no longer be used. In C++, you must release references to deleted <b>IAzTask</b> objects by calling the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nf-unknwn-iunknown-release">IUnknown::Release</a> method. In Visual Basic, references to deleted objects are automatically released.



