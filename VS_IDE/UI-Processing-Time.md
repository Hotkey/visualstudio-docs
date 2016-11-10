---
title: "UI Processing Time"
ms.custom: na
ms.date: 10/03/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-debug
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 0ddb05a3-8c6b-448b-8488-2751c1e5abcc
caps.latest.revision: 5
manager: ghogen
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# UI Processing Time
These segments in the timeline are associated with blocking times that are categorized as UI Processing. This implies that a thread is pumping Windows messages or performing other user interface (UI) work. During this time, a thread has been blocked in an API that the Concurrency Visualizer is counting as UI Processing. APIs such as `GetMessage()` and `MsgWaitForMultipleObjects()` fall into this group.  
  
 If no pre-defined blocking API is identified, review the call stacks and profile reports to determine the underlying causes of delay.  
  
 The UI Processing category is important for understanding the responsiveness of GUI applications, and is desirable in applications that depend on UI responsiveness. For example, if the UI thread in an application achieves 100% time in UI Processing, it is probably very responsive. However, if the UI thread spends considerable time in other categories, look for the root causes and consider options for reducing non-UI categories on that thread.  
  
## See Also  
 [Threads View](../VS_IDE/Threads-View--Parallel-Performance-.md)