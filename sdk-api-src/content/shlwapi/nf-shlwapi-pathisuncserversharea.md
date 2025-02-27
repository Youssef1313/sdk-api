---
UID: NF:shlwapi.PathIsUNCServerShareA
title: PathIsUNCServerShareA function (shlwapi.h)
description: Determines if a string is a valid Universal Naming Convention (UNC) share path, \\server\share.
old-location: shell\PathIsUNCServerShare.htm
tech.root: shell
ms.assetid: 306cfc34-7cb2-4f60-af5c-8b567149c2fc
ms.date: 12/05/2018
ms.keywords: PathIsUNCServerShare, PathIsUNCServerShare function [Windows Shell], PathIsUNCServerShareA, PathIsUNCServerShareW, _win32_PathIsUNCServerShare, shell.PathIsUNCServerShare, shlwapi/PathIsUNCServerShare, shlwapi/PathIsUNCServerShareA, shlwapi/PathIsUNCServerShareW
ms.topic: function
f1_keywords:
- shlwapi/PathIsUNCServerShare
dev_langs:
- c++
req.header: shlwapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: PathIsUNCServerShareW (Unicode) and PathIsUNCServerShareA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Shlwapi.lib
req.dll: Shlwapi.dll (version 4.71 or later)
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Shlwapi.dll
- API-MS-Win-Core-shlwapi-legacy-l1-1-0.dll
- KernelBase.dll
- API-MS-Win-DownLevel-shlwapi-l1-1-0.dll
- API-MS-Win-DownLevel-shlwapi-l1-1-1.dll
api_name:
- PathIsUNCServerShare
- PathIsUNCServerShareA
- PathIsUNCServerShareW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# PathIsUNCServerShareA function


## -description


Determines if a string is a valid Universal Naming Convention (UNC) share path, \\<i>server</i>\<i>share</i>.


## -parameters




### -param pszPath [in]

Type: <b>LPCTSTR</b>

A pointer to a null-terminated string of maximum length MAX_PATH that contains the path to be validated.


## -returns



Type: <b>BOOL</b>

Returns <b>TRUE</b> if the string is in the form \\<i>server</i>\<i>share</i>, or <b>FALSE</b> otherwise.



