---
title: "IDebugArrayObject2::GetBaseIndices | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "GetBaseIndices"
  - "IDebugArrayObject2::GetBaseIndices"
ms.assetid: 882951a2-3da0-49bf-8d1e-7daedd13ffe6
caps.latest.revision: 9
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugArrayObject2::GetBaseIndices
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugArrayObject2::GetBaseIndices](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugarrayobject2-getbaseindices).  
  
Retrieves the base indices (lower bounds) for each index given the number of dimensions in the array.  
  
## Syntax  
  
```cpp#  
HRESULT GetBaseIndices (  
   DWORD  dwRank,  
   DWORD* dwIndices  
);  
```  
  
```csharp  
int GetBaseIndices (  
   uint       dwRank,  
   out uint[] dwIndices  
);  
```  
  
#### Parameters  
 `dwRank`  
 [in] The number of dimensions (rank) of the array.  
  
 `dwIndices`  
 [out] The base indices (lower bounds) for the array.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 As an example, this function would return ‘5’ for the array created by the following C# code:  
  
```  
int[] lengths = { 12 };  
int[] lowerbounds = { 5 };  
Array.CreateInstance(typeof(int), lengths, lowerbounds);  
```  
  
## See Also  
 [IDebugArrayObject2](../../../extensibility/debugger/reference/idebugarrayobject2.md)

