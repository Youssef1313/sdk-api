---
UID: NF:mfspatialaudio.IMFSpatialAudioSample.AddSpatialAudioObject
title: IMFSpatialAudioSample::AddSpatialAudioObject (mfspatialaudio.h)
description: Adds a new spatial audio object, represented by an IMFSpatialAudioObjectBuffer object, to the sample.
old-location: mf\imfspatialaudiosample_addspatialaudioobject.htm
tech.root: medfound
ms.assetid: D967B4FE-8E11-4520-BF9E-725ACC7AA99A
ms.date: 12/05/2018
ms.keywords: AddSpatialAudioObject, AddSpatialAudioObject method [Media Foundation], AddSpatialAudioObject method [Media Foundation],IMFSpatialAudioSample interface, IMFSpatialAudioSample interface [Media Foundation],AddSpatialAudioObject method, IMFSpatialAudioSample.AddSpatialAudioObject, IMFSpatialAudioSample::AddSpatialAudioObject, mf.imfspatialaudiosample_addspatialaudioobject, mfspatialaudio/IMFSpatialAudioSample::AddSpatialAudioObject
ms.topic: method
f1_keywords:
- mfspatialaudio/IMFSpatialAudioSample.AddSpatialAudioObject
dev_langs:
- c++
req.header: mfspatialaudio.h
req.include-header: Mfobjects.h
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1703 [desktop apps only]
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
req.lib: Mfobjects.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- mfobjects.lib
- mfobjects.dll
api_name:
- IMFSpatialAudioSample.AddSpatialAudioObject
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFSpatialAudioSample::AddSpatialAudioObject


## -description


Adds a new spatial audio object, represented by an <a href="https://docs.microsoft.com/windows/desktop/api/mfspatialaudio/nn-mfspatialaudio-imfspatialaudioobjectbuffer">IMFSpatialAudioObjectBuffer</a> object, to the     sample.


## -parameters




### -param pAudioObjBuffer [in]

A pointer to the new IMFSpatialAudioObject.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The supplied pointer is invalid.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mfspatialaudio/nn-mfspatialaudio-imfspatialaudiosample">IMFSpatialAudioSample</a>
 

 

