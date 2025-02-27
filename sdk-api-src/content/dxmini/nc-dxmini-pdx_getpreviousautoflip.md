---
UID: NC:dxmini.PDX_GETPREVIOUSAUTOFLIP
title: PDX_GETPREVIOUSAUTOFLIP (dxmini.h)
description: The DxGetPreviousAutoflip callback function is called when the device is hardware autoflipping and a client of the video miniport driver wants to know which surface received the previous field of video data for capture purposes.
old-location: display\dxgetpreviousautoflip.htm
tech.root: display
ms.assetid: 3b19e4be-413c-4014-b414-cb2ba3e14b14
ms.date: 12/05/2018
ms.keywords: DxGetPreviousAutoflip, DxGetPreviousAutoflip callback function [Display Devices], PDX_GETPREVIOUSAUTOFLIP, PDX_GETPREVIOUSAUTOFLIP callback, VideoMiniPort_DxApiFunctions_07351af6-3fdc-4a60-852f-23ea28bc6e2b.xml, display.dxgetpreviousautoflip, dxmini/DxGetPreviousAutoflip
ms.topic: callback
f1_keywords:
- dxmini/DxGetPreviousAutoflip
dev_langs:
- c++
req.header: dxmini.h
req.include-header: Dxmini.h
req.target-type: Desktop
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
- UserDefined
api_location:
- dxmini.h
api_name:
- DxGetPreviousAutoflip
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# PDX_GETPREVIOUSAUTOFLIP callback function


## -description


The<i> DxGetPreviousAutoflip</i> callback function is called when the device is hardware autoflipping and a client of the video miniport driver wants to know which surface received the previous field of video data for capture purposes. 


## -parameters




### -param Arg1


### -param Arg2


### -param Arg3








#### - GetPreviousAutoflipInInfo

Points to a <a href="https://docs.microsoft.com/windows/desktop/api/dxmini/ns-dxmini-ddgetpreviousautoflipininfo">DDGETPREVIOUSAUTOFLIPININFO</a> structure that contains the <a href="https://docs.microsoft.com/windows-hardware/drivers/">video port extensions (VPE)</a> object information.


#### - GetPreviousAutoflipOutInfo

Points to a <a href="https://docs.microsoft.com/windows/desktop/api/dxmini/ns-dxmini-ddgetpreviousautoflipoutinfo">DDGETPREVIOUSAUTOFLIPOUTINFO</a> structure that contains the index of the autoflip chain.


#### - HwDeviceExtension

Points to the miniport driver's device extension.


## -returns



<i>DxGetPreviousAutoflip</i> returns DX_OK if it succeeds; otherwise, it returns one of the following error values:




## -remarks



If interleaving, the surface that received the previous field may be the same surface that is receiving the current field. 

<i>DxGetPreviousAutoflip</i> returns the index in the autoflip chain of the correct surface in the <b>dwSurfaceIndex</b> member of the DDGETPREVIOUSAUTOFLIPOUTINFO structure at <i>GetPreviousAutoflipOutInfo</i>. 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/dxmini/ns-dxmini-ddgetpreviousautoflipininfo">DDGETPREVIOUSAUTOFLIPININFO</a>



<a href="https://docs.microsoft.com/windows/desktop/api/dxmini/ns-dxmini-ddgetpreviousautoflipoutinfo">DDGETPREVIOUSAUTOFLIPOUTINFO</a>
 

 

