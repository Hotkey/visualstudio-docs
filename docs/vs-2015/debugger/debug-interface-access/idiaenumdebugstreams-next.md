---
title: "IDiaEnumDebugStreams::Next | Microsoft Docs"
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
  - "IDiaEnumDebugStreams::Next method"
ms.assetid: eb8eae5a-be27-45f4-a7bd-6e4ef0652385
caps.latest.revision: 10
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaEnumDebugStreams::Next
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaEnumDebugStreams::Next](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiaenumdebugstreams-next).  
  
Retrieves a specified number of debug streams in the enumeration sequence.  
  
## Syntax  
  
```cpp#  
HRESULT Next (   
   ULONG                     celt,   
   IDiaEnumDebugStreamData** rgelt,  
   ULONG*                    pceltFetched  
);  
```  
  
#### Parameters  
 celt  
 [in] **T**he number of debug streams in the enumerator to be retrieved.  
  
 rgelt  
 [out] Returns an array of [IDiaEnumDebugStreamData](../../debugger/debug-interface-access/idiaenumdebugstreamdata.md) objects that represents the debug streams being retrieved.  
  
 pceltFetched  
 [out] Returns the number of debug streams returned.  
  
## Return Value  
 If successful, returns `S_OK`. Returns `S_FALSE` if there are no more streams. Otherwise, returns an error code.  
  
## See Also  
 [IDiaEnumDebugStreams](../../debugger/debug-interface-access/idiaenumdebugstreams.md)



