---
UID: NS:strmif.tagDVD_VideoAttributes
title: DVD_VideoAttributes (strmif.h)
description: The DVD_VideoAttributes structure describes the attributes of the video stream for the current title or menu.
old-location: dshow\dvd_videoattributes.htm
tech.root: DirectShow
ms.assetid: b395a322-d63e-41a0-b97a-88f99aeba0e5
ms.date: 12/05/2018
ms.keywords: DVD_VideoAttributes, DVD_VideoAttributes structure [DirectShow], DVD_VideoAttributesStructure, dshow.dvd_videoattributes, strmif/DVD_VideoAttributes
ms.topic: struct
f1_keywords:
- strmif/DVD_VideoAttributes
dev_langs:
- c++
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
- strmif.h
api_name:
- DVD_VideoAttributes
targetos: Windows
req.typenames: DVD_VideoAttributes
req.redist: 
ms.custom: 19H1
---

# DVD_VideoAttributes structure


## -description



The <code>DVD_VideoAttributes</code> structure describes the attributes of the video stream for the current title or menu.




## -struct-fields




### -field fPanscanPermitted

<b>TRUE</b> means the picture can be shown as pan-scan if the display aspect ratio is 4 x 3.


### -field fLetterboxPermitted

<b>TRUE</b> means the picture can be shown as letterbox if the display aspect ratio is 4 x 3.


### -field ulAspectX

The video stream's X aspect (4 or 16).


### -field ulAspectY

The video stream's Y aspect (3 or 9).


### -field ulFrameRate

The frame rate in hertz (Hz), either 50 or 60.


### -field ulFrameHeight

The frame height in lines (525 for a frame rate of 60 Hz or 625 for 50 Hz).


### -field Compression

Variable of type <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/strmif/ne-strmif-dvd_video_compression">DVD_VIDEO_COMPRESSION</a> indicating the MPEG compression type used on the disc.


### -field fLine21Field1InGOP

<b>TRUE</b> means there is user data in line 21, field 1.


### -field fLine21Field2InGOP

<b>TRUE</b> means there is user data in line 21, field 2.


### -field ulSourceResolutionX

The x-axis source resolution (352, 704, or 720).


### -field ulSourceResolutionY

The y-axis source resolution (240, 480, 288, or 576).


### -field fIsSourceLetterboxed

<b>TRUE</b> means the source video is in letterbox format. Subpictures and menu buttons can only be displayed in the active video area.


### -field fIsFilmMode

For 625/50 Hz systems, <b>TRUE</b> means "film mode" and <b>FALSE</b> means "camera mode."


## -remarks



This structure is filled when an application calls the <a href="https://docs.microsoft.com/windows/desktop/api/strmif/nf-strmif-idvdinfo2-getcurrentvideoattributes">IDvdInfo2::GetCurrentVideoAttributes</a> method.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/DirectShow/directshow-structures">DirectShow Structures</a>
 

 

