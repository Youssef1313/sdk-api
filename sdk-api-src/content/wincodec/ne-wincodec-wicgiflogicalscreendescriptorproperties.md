---
UID: NE:wincodec.WICGifLogicalScreenDescriptorProperties
title: WICGifLogicalScreenDescriptorProperties (wincodec.h)
description: Specifies the logical screen descriptor properties for Graphics Interchange Format (GIF) metadata.
old-location: wic\_wic_codec_wicgiflogicalscreendescriptorproperties.htm
tech.root: wic
ms.assetid: edeaae2d-ba4a-4d03-b1ce-37bb5cd67e03
ms.date: 12/05/2018
ms.keywords: WICGifLogicalScreenDescriptorBackgroundColorIndex, WICGifLogicalScreenDescriptorColorResolution, WICGifLogicalScreenDescriptorGlobalColorTableFlag, WICGifLogicalScreenDescriptorGlobalColorTableSize, WICGifLogicalScreenDescriptorHeight, WICGifLogicalScreenDescriptorPixelAspectRatio, WICGifLogicalScreenDescriptorProperties, WICGifLogicalScreenDescriptorProperties enumeration [Windows Imaging Component], WICGifLogicalScreenDescriptorSortFlag, WICGifLogicalScreenDescriptorWidth, WICGifLogicalScreenSignature, _wic_codec_wicgiflogicalscreendescriptorproperties, wic._wic_codec_wicgiflogicalscreendescriptorproperties, wincodec/WICGifLogicalScreenDescriptorBackgroundColorIndex, wincodec/WICGifLogicalScreenDescriptorColorResolution, wincodec/WICGifLogicalScreenDescriptorGlobalColorTableFlag, wincodec/WICGifLogicalScreenDescriptorGlobalColorTableSize, wincodec/WICGifLogicalScreenDescriptorHeight, wincodec/WICGifLogicalScreenDescriptorPixelAspectRatio, wincodec/WICGifLogicalScreenDescriptorProperties, wincodec/WICGifLogicalScreenDescriptorSortFlag, wincodec/WICGifLogicalScreenDescriptorWidth, wincodec/WICGifLogicalScreenSignature
ms.topic: enum
f1_keywords:
- wincodec/WICGifLogicalScreenDescriptorProperties
dev_langs:
- c++
req.header: wincodec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wincodec.idl
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
- Wincodec.h
api_name:
- WICGifLogicalScreenDescriptorProperties
targetos: Windows
req.typenames: WICGifLogicalScreenDescriptorProperties
req.redist: 
ms.custom: 19H1
---

# WICGifLogicalScreenDescriptorProperties enumeration


## -description


Specifies the logical screen descriptor properties for Graphics Interchange Format (GIF) metadata.


## -enum-fields




### -field WICGifLogicalScreenSignature

 [VT_UI1 | VT_VECTOR] Indicates the signature property.


### -field WICGifLogicalScreenDescriptorWidth

[VT_UI2] Indicates the width in pixels. 


### -field WICGifLogicalScreenDescriptorHeight

[VT_UI2] Indicates the height in pixels. 


### -field WICGifLogicalScreenDescriptorGlobalColorTableFlag

[VT_BOOL] Indicates the  global color table flag. <b>TRUE</b> if a global color table is present; otherwise, <b>FALSE</b>.


### -field WICGifLogicalScreenDescriptorColorResolution

[VT_UI1] Indicates the color resolution in bits per pixel.


### -field WICGifLogicalScreenDescriptorSortFlag

[VT_BOOL] Indicates the sorted color table flag. <b>TRUE</b> if the table is sorted; otherwise, <b>FALSE</b>.


### -field WICGifLogicalScreenDescriptorGlobalColorTableSize

[VT_UI1] Indicates the value used to calculate the number of bytes contained in the global color table. 

To calculate the actual size of the color table, raise 2 to the value of the field + 1.


### -field WICGifLogicalScreenDescriptorBackgroundColorIndex

[VT_UI1] Indicates the index within the color table to use for the background (pixels not defined in the image).


### -field WICGifLogicalScreenDescriptorPixelAspectRatio

[VT_UI1] Indicates the factor used to compute an approximation of the aspect ratio.


### -field WICGifLogicalScreenDescriptorProperties_FORCE_DWORD



