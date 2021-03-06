---
title: "IDebugEngine3::LoadSymbols | Microsoft Docs"
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
  - "IDebugEngine3::LoadSymbols"
helpviewer_keywords: 
  - "IDebugEngine3::LoadSymbols"
ms.assetid: c846a440-1d91-4d48-b8f1-82e902ae152b
caps.latest.revision: 8
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugEngine3::LoadSymbols
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugEngine3::LoadSymbols](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugengine3-loadsymbols).  
  
Loads (as necessary) symbols for all modules being debugged by this debugging engine.  
  
## Syntax  
  
```cpp  
HRESULT LoadSymbols();  
```  
  
```csharp  
int LoadSymbols();  
```  
  
#### Parameters  
 None.  
  
## Return Value  
 If successful, returns S_OK; otherwise returns error code.  
  
## Remarks  
 This loads debugging symbols for all modules referenced by this debugging engine. The symbols are loaded only if they have not already been loaded. Symbols are searched on the paths set by a call to [SetSymbolPath](../../../extensibility/debugger/reference/idebugengine3-setsymbolpath.md).  
  
## See Also  
 [SetSymbolPath](../../../extensibility/debugger/reference/idebugengine3-setsymbolpath.md)   
 [IDebugEngine3](../../../extensibility/debugger/reference/idebugengine3.md)

