---
UID: NF:evr.IMFVideoMixerControl.GetStreamOutputRect
title: IMFVideoMixerControl::GetStreamOutputRect (evr.h)
description: Retrieves the position of a video stream within the composition rectangle.
old-location: mf\imfvideomixercontrol_getstreamoutputrect.htm
tech.root: medfound
ms.assetid: 6de631cd-f85e-4f53-b14c-8ca3cd65b719
ms.date: 12/05/2018
ms.keywords: 6de631cd-f85e-4f53-b14c-8ca3cd65b719, GetStreamOutputRect, GetStreamOutputRect method [Media Foundation], GetStreamOutputRect method [Media Foundation],IMFVideoMixerControl interface, IMFVideoMixerControl interface [Media Foundation],GetStreamOutputRect method, IMFVideoMixerControl.GetStreamOutputRect, IMFVideoMixerControl::GetStreamOutputRect, evr/IMFVideoMixerControl::GetStreamOutputRect, mf.imfvideomixercontrol_getstreamoutputrect
ms.topic: method
f1_keywords:
- evr/IMFVideoMixerControl.GetStreamOutputRect
dev_langs:
- c++
req.header: evr.h
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
api_name:
- IMFVideoMixerControl.GetStreamOutputRect
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFVideoMixerControl::GetStreamOutputRect


## -description



Retrieves the position of a video stream within the composition rectangle.




## -parameters




### -param dwStreamID [in]

The identifier of the stream. For the EVR media sink, the stream identifier is defined when the <a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nf-mfidl-imfmediasink-addstreamsink">IMFMediaSink::AddStreamSink</a> method is called. For the DirectShow EVR filter, the stream identifier corresponds to the pin index. The reference stream is always stream 0.


### -param pnrcOutput [out]

Pointer to an <a href="https://docs.microsoft.com/windows/desktop/api/evr/ns-evr-mfvideonormalizedrect">MFVideoNormalizedRect</a> structure that receives the bounding rectangle, in normalized coordinates.


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
<dt><b>MF_E_INVALIDSTREAMNUMBER</b></dt>
</dl>
</td>
<td width="60%">
Invalid stream identifier.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/medfound/enhanced-video-renderer">Enhanced Video Renderer</a>



<a href="https://docs.microsoft.com/windows/desktop/api/evr/nn-evr-imfvideomixercontrol">IMFVideoMixerControl</a>
 

 

