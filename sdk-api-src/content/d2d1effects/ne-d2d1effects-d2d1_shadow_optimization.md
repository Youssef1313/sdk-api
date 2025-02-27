---
UID: NE:d2d1effects.D2D1_SHADOW_OPTIMIZATION
title: D2D1_SHADOW_OPTIMIZATION (d2d1effects.h)
description: The level of performance optimization for the Shadow effect.
old-location: direct2d\d2d1_shadow_optimization.htm
tech.root: Direct2D
ms.assetid: 1C509608-BEBA-4E4C-8EC5-88B587D81B34
ms.date: 12/05/2018
ms.keywords: D2D1_SHADOW_OPTIMIZATION, D2D1_SHADOW_OPTIMIZATION enumeration [Direct2D], D2D1_SHADOW_OPTIMIZATION_BALANCED, D2D1_SHADOW_OPTIMIZATION_QUALITY, D2D1_SHADOW_OPTIMIZATION_SPEED, d2d1effects/D2D1_SHADOW_OPTIMIZATION, d2d1effects/D2D1_SHADOW_OPTIMIZATION_BALANCED, d2d1effects/D2D1_SHADOW_OPTIMIZATION_QUALITY, d2d1effects/D2D1_SHADOW_OPTIMIZATION_SPEED, direct2d.d2d1_shadow_optimization
ms.topic: enum
f1_keywords:
- d2d1effects/D2D1_SHADOW_OPTIMIZATION
dev_langs:
- c++
req.header: d2d1effects.h
req.include-header: 
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
- d2d1effects.h
api_name:
- D2D1_SHADOW_OPTIMIZATION
targetos: Windows
req.typenames: D2D1_SHADOW_OPTIMIZATION
req.redist: 
ms.custom: 19H1
---

# D2D1_SHADOW_OPTIMIZATION enumeration


## -description


The level of performance optimization for the <a href="https://docs.microsoft.com/windows/desktop/Direct2D/drop-shadow">Shadow effect</a>.


## -enum-fields




### -field D2D1_SHADOW_OPTIMIZATION_SPEED

Applies internal optimizations such as pre-scaling at relatively small radii. Uses linear filtering.


### -field D2D1_SHADOW_OPTIMIZATION_BALANCED

Uses the same optimization thresholds as Speed mode, but uses trilinear filtering.


### -field D2D1_SHADOW_OPTIMIZATION_QUALITY

Only uses internal optimizations with large blur radii, where approximations are less likely to be visible. Uses trilinear filtering.


### -field D2D1_SHADOW_OPTIMIZATION_FORCE_DWORD



