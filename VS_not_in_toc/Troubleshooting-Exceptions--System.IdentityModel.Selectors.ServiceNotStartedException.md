---
title: "Troubleshooting Exceptions: System.IdentityModel.Selectors.ServiceNotStartedException"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 6d34bab2-994a-4b0c-893d-19b5d7acf92d
caps.latest.revision: 14
manager: douge
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# Troubleshooting Exceptions: System.IdentityModel.Selectors.ServiceNotStartedException
A <xref:System.IdentityModel.Selectors.ServiceNotStartedException?qualifyHint=False> exception is thrown when CardSpace has not been started on the user's computer. If CardSpace has attempted to start but has been unable to for any reason, this exception is thrown.  
  
 Check that the CardSpace service is installed and enabled on the computer. Try to start the CardSpace service manually by using Microsoft Management Console (MMC).  
  
 CardSpace version 1 does not support FAT file systems. On FAT systems, CardSpace will not start and this exception will occur.  
  
## See Also  
 <xref:System.IdentityModel.Selectors.ServiceNotStartedException?qualifyHint=False>   
 [Use the Exception Assistant](../Topic/How%20to:%20Use%20the%20Exception%20Assistant.md)