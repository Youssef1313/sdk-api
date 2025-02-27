---
UID: NN:wmcontainer.IMFASFStreamConfig
title: IMFASFStreamConfig (wmcontainer.h)
description: Configures the settings of a stream in an ASF file.
old-location: mf\imfasfstreamconfig.htm
tech.root: medfound
ms.assetid: 7bb63396-21c2-400d-b9de-c00b90f46d62
ms.date: 12/05/2018
ms.keywords: 7bb63396-21c2-400d-b9de-c00b90f46d62, IMFASFStreamConfig, IMFASFStreamConfig interface [Media Foundation], IMFASFStreamConfig interface [Media Foundation],described, mf.imfasfstreamconfig, wmcontainer/IMFASFStreamConfig
ms.topic: interface
f1_keywords:
- wmcontainer/IMFASFStreamConfig
dev_langs:
- c++
req.header: wmcontainer.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- mfuuid.lib
- mfuuid.dll
api_name:
- IMFASFStreamConfig
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFASFStreamConfig interface


## -description


Configures the settings of a stream in an ASF file. The ASF stream configuration object exposes this interface. To obtain a pointer to this interface, call the <a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfprofile-createstream">IMFASFProfile::CreateStream</a> method.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMFASFStreamConfig</b> interface inherits from <a href="https://docs.microsoft.com/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes">IMFAttributes</a>. <b>IMFASFStreamConfig</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMFASFStreamConfig</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-addpayloadextension">AddPayloadExtension</a>
</td>
<td align="left" width="63%">
Configures a payload extension for the stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-clone">Clone</a>
</td>
<td align="left" width="63%">
Creates a copy of the ASF stream configuration object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-getmediatype">GetMediaType</a>
</td>
<td align="left" width="63%">
Retrieves the media type of the stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-getpayloadextension">GetPayloadExtension</a>
</td>
<td align="left" width="63%">
Retrieves information about an existing payload extension.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-getpayloadextensioncount">GetPayloadExtensionCount</a>
</td>
<td align="left" width="63%">
Retrieves the number of payload extensions that are configured for the stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-getstreamnumber">GetStreamNumber</a>
</td>
<td align="left" width="63%">
Retrieves the stream number of the stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-getstreamtype">GetStreamType</a>
</td>
<td align="left" width="63%">
Retrieves the major media type of the stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-removeallpayloadextensions">RemoveAllPayloadExtensions</a>
</td>
<td align="left" width="63%">
Removes all payload extensions that are configured for the stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-setmediatype">SetMediaType</a>
</td>
<td align="left" width="63%">
Sets the media type for the ASF stream configuration object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfstreamconfig-setstreamnumber">SetStreamNumber</a>
</td>
<td align="left" width="63%">
Assigns a stream number to the stream.

</td>
</tr>
</table> 


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes">IMFAttributes</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/media-foundation-interfaces">Media Foundation Interfaces</a>
 

 

