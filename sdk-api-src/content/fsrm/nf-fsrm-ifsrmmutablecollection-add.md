---
UID: NF:fsrm.IFsrmMutableCollection.Add
title: IFsrmMutableCollection::Add (fsrm.h)
description: Adds an object to the collection.
old-location: fsrm\ifsrmmutablecollection_add.htm
tech.root: fsrm
ms.assetid: 916f01de-c87c-450c-859a-c349a165f91d
ms.date: 12/05/2018
ms.keywords: Add, Add method [File Server Resource Manager], Add method [File Server Resource Manager],IFsrmMutableCollection interface, IFsrmMutableCollection interface [File Server Resource Manager],Add method, IFsrmMutableCollection.Add, IFsrmMutableCollection::Add, fs.ifsrmmutablecollection_add, fsrm.ifsrmmutablecollection_add, fsrm/IFsrmMutableCollection::Add
ms.topic: method
f1_keywords:
- fsrm/IFsrmMutableCollection.Add
dev_langs:
- c++
req.header: fsrm.h
req.include-header: FsrmQuota.h, FsrmReports.h, FsrmScreen.h
req.target-type: Windows
req.target-min-winverclnt: None supported
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
req.dll: SrmSvc.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- SrmSvc.dll
api_name:
- IFsrmMutableCollection.Add
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFsrmMutableCollection::Add


## -description


Adds an object to the collection.


## -parameters




### -param item [in]

A <b>VARIANT</b> that contains the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/oaidl/nn-oaidl-idispatch">IDispatch</a> interface of the object to add to the collection. Set the variant type to <b>VT_DISPATCH</b> and the <b>pdispVal</b> member to the <b>IDispatch</b> interface of the object.


## -returns



The method returns the following return values.




## -remarks



All items in the collection must be of the same type.


#### Examples

For an example, see <a href="https://docs.microsoft.com/previous-versions/windows/desktop/fsrm/using-templates-to-define-file-screens">Using Templates to Define File Screens</a>.

<div class="code"></div>



## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/fsrm/nn-fsrm-ifsrmmutablecollection">IFsrmMutableCollection</a>
 

 

