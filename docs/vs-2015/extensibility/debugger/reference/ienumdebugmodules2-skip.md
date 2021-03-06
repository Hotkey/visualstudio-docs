---
title: "IEnumDebugModules2::Skip | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IEnumDebugModules2::Skip"
helpviewer_keywords: 
  - "IEnumDebugModules2::Skip"
ms.assetid: 61dc42f4-8544-45bb-8da0-fb22cccec7da
caps.latest.revision: 10
ms.author: "gregvanl"
manager: "ghogen"
---
# IEnumDebugModules2::Skip
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IEnumDebugModules2::Skip](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/ienumdebugmodules2-skip).  
  
Skips over the specified number of elements.  
  
## Syntax  
  
```cpp#  
HRESULT Skip(  
   ULONG celt  
);  
```  
  
```csharp  
int Skip(  
   uint celt  
);  
```  
  
#### Parameters  
 `celt`  
 [in] Number of elements to skip.  
  
## Return Value  
 If successful, returns `S_OK`. Returns `S_FALSE` if `celt` is greater than the number of remaining elements; otherwise, returns an error code.  
  
## Remarks  
 If `celt` specifies a value greater than the number of remaining elements, the enumeration is set to the end and `S_FALSE` is returned.  
  
## See Also  
 [IEnumDebugModules2](../../../extensibility/debugger/reference/ienumdebugmodules2.md)

