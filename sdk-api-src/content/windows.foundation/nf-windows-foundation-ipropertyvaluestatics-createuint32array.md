---
UID: NF:windows.foundation.IPropertyValueStatics.CreateUInt32Array
title: IPropertyValueStatics::IPropertyValueStatics (windows.foundation.h)
description: Creates a new IPropertyValue object that contains the specified array of unsigned 32-bit integer values.
old-location: winrt\ipropertyvaluestatics_createuint32array.htm
tech.root: WinRT
ms.assetid: 0f56b855-a116-4c58-ae93-1a3d49240685
ms.date: 12/05/2018
ms.keywords: CreateUInt32Array, CreateUInt32Array method [Windows Runtime], CreateUInt32Array method [Windows Runtime],IPropertyValueStatics interface, IPropertyValueStatics interface [Windows Runtime],CreateUInt32Array method, IPropertyValueStatics.CreateUInt32Array, IPropertyValueStatics.IPropertyValueStatics, IPropertyValueStatics::CreateUInt32Array, IPropertyValueStatics::IPropertyValueStatics, windows/IPropertyValueStatics::CreateUInt32Array, winrt.ipropertyvaluefactory_createuint32array, winrt.ipropertyvaluestatics_createuint32array
ms.topic: method
f1_keywords:
- windows.foundation/IPropertyValueStatics.CreateUInt32Array
dev_langs:
- c++
req.header: windows.foundation.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Windows.Foundation.idl
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
- Windows.Foundation.h
api_name:
- IPropertyValueStatics.CreateUInt32Array
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPropertyValueStatics::IPropertyValueStatics


## -description


Creates a new <a href="https://docs.microsoft.com/windows/desktop/api/windows.foundation/nn-windows-foundation-ipropertyvalue">IPropertyValue</a> object that contains  the specified array of unsigned 32-bit integer values.


## -parameters




### -param __valueSize [in]

Type: <b>UINT32</b>

The number of values in the array.


### -param value [in]

Type: <b>UINT32*</b>

The array of unsigned 32-bit integer values to store.


### -param propertyValue [out, retval]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/inspectable/nn-inspectable-iinspectable">IInspectable</a>**</b>

A pointer to a new object that contains <i>value</i>. Use the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nf-unknwn-iunknown-queryinterface(q_)">IUnknown::QueryInterface</a> method to get the <a href="https://docs.microsoft.com/windows/desktop/api/windows.foundation/nn-windows-foundation-ipropertyvalue">IPropertyValue</a> interface for the object.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/windows.foundation/nf-windows-foundation-ipropertyvalue-getuint32array">IPropertyValue::GetUInt32Array</a>



<a href="https://docs.microsoft.com/windows/desktop/api/windows.foundation/nn-windows-foundation-ipropertyvaluestatics">IPropertyValueStatics</a>
 

 

