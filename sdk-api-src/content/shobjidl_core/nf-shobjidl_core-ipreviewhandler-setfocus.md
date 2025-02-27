---
UID: NF:shobjidl_core.IPreviewHandler.SetFocus
title: IPreviewHandler::SetFocus (shobjidl_core.h)
description: Directs the preview handler to set focus to itself.
old-location: shell\IPreviewHandler_SetFocus.htm
tech.root: shell
ms.assetid: 93667383-da56-4fe9-a79e-933ab9703365
ms.date: 12/05/2018
ms.keywords: IPreviewHandler interface [Windows Shell],SetFocus method, IPreviewHandler.SetFocus, IPreviewHandler::SetFocus, SetFocus, SetFocus method [Windows Shell], SetFocus method [Windows Shell],IPreviewHandler interface, _shell_IPreviewHandler_SetFocus, shell.IPreviewHandler_SetFocus, shobjidl_core/IPreviewHandler::SetFocus
ms.topic: method
f1_keywords:
- shobjidl_core/IPreviewHandler.SetFocus
dev_langs:
- c++
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
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
- COM
api_location:
- shobjidl_core.h
api_name:
- IPreviewHandler.SetFocus
targetos: Windows
req.typenames: 
req.redist: Windows Search 4 or later
ms.custom: 19H1
---

# IPreviewHandler::SetFocus


## -description


Directs the preview handler to set focus to itself.


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This method should query the state of the <b>SHIFT</b> key to decide whether to set focus to its first tab stop or its last tab stop. This is necessary because the <b>IPreviewHandler::SetFocus</b> can only succeed if the focus is being set to a window created by the calling thread.

This is the extent of accelerator keys coming down from the host to the preview handler; no other accelerators are passed down. <a href="https://docs.microsoft.com/windows/desktop/api/shobjidl_core/nf-shobjidl_core-ipreviewhandler-translateaccelerator">IPreviewHandler::TranslateAccelerator</a> is only used for messages from the preview handler's message pump up to the <a href="https://docs.microsoft.com/windows/desktop/api/shobjidl_core/nn-shobjidl_core-ipreviewhandler">IPreviewHandler</a> object.



