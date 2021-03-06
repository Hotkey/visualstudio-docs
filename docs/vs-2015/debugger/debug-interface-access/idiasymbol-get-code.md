---
title: "IDiaSymbol::get_code | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "IDiaSymbol::get_code method"
ms.assetid: 5f425fa3-7ba6-4979-8b3e-0fcd06cbba73
caps.latest.revision: 11
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaSymbol::get_code
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaSymbol::get_code](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiasymbol-get-code).  
  
Retrieves a flag that specifies whether the symbol refers to a code address.  
  
## Syntax  
  
```cpp#  
HRESULT get_code (   
   BOOL* pRetVal  
);  
```  
  
#### Parameters  
 `pRetVal`  
 [out] Returns `TRUE` if the symbol refers to a code address, otherwise, returns `FALSE`.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or error code.  
  
> [!NOTE]
>  A return value of `S_FALSE` means the property is not available for the symbol.  
  
## Requirements  
  
|Requirement|Description|  
|-----------------|-----------------|  
|Header:|dia2.h|  
|Version:|DIA SDK v7.0|  
  
## See Also  
 [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)



