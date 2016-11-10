---
title: "TransactedReceiveScope Activity Designer"
ms.custom: na
ms.date: "10/02/2016"
ms.prod: ".net-framework-4.6"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "reference"
f1_keywords: 
  - "System.ServiceModel.Activities.TransactedReceiveScope.UI"
ms.assetid: 7ca93aad-4e83-4d81-90f4-998ee114d9b6
caps.latest.revision: 4
ms.author: "erikre"
manager: "erikre"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# TransactedReceiveScope Activity Designer
The **TransactedReceiveScope** designer is used to create and configure a \<xref:System.ServiceModel.Activities.TransactedReceiveScope> activity.  
  
## The TransactedReceiveScope Activity  
 The \<xref:System.ServiceModel.Activities.TransactedReceiveScope> activity enables you to flow a transaction into server transactions created by a workflow or dispatcher.  
  
### Using the TransactedReceiveScope Activity Designer  
 The **TransactedReceiveScope** activity designer can be found in the **Messaging** category of the **Toolbox**, which is accessed by clicking the **Toolbox** tab on [!INCLUDE[wfd2](../workflowdesigner/includes/wfd2_md.md)] (Alternatively, select **Toolbar** from the **View** menu, or CTRL+ALT+X.)  
  
 The **TransactedReceiveScope** activity designer can be dragged from the **Toolbox** and dropped on to the [!INCLUDE[wfd2](../workflowdesigner/includes/wfd2_md.md)] surface wherever activities are usually placed. This creates a \<xref:System.ServiceModel.Activities.TransactedReceiveScope> activity with a default **DisplayName** of TransactedReceiveScope. The \<xref:System.Activities.Activity.DisplayName*> can be edited in the header of the **TransactedReceiveScope** activity designer or in the **DisplayName** box of the property grid.  
  
 The **TransactedReceiveScope** designer contains **Request** and **Body** boxes. These are used to configure the \<xref:System.ServiceModel.Activities.TransactedReceiveScope.Request*> property, which specifies a \<xref:System.ServiceModel.Activities.Receive> activity and a \<xref:System.ServiceModel.Activities.TransactedReceiveScope.Body*> property, which specifies some other \<xref:System.Activities.Activity>. The \<xref:System.ServiceModel.Activities.TransactedReceiveScope.Request*> creates a transaction. The transaction then is made ambient for the scope of the \<xref:System.ServiceModel.Activities.TransactedReceiveScope.Body*> so that any activity within this scope executes inside this transaction.  
  
### The TransactedReceiveScope Properties  
 The following table shows the \<xref:System.ServiceModel.Activities.TransactedReceiveScope> properties and describes how they are used in the designer. These \<xref:System.Activities.Activity.DisplayName*> property can be edited in property grid or on the [!INCLUDE[wfd2](../workflowdesigner/includes/wfd2_md.md)] surface, but the others must be edited on the design surface.  
  
|Property Name|Required|Usage|  
|-------------------|--------------|-----------|  
|\<xref:System.Activities.Activity.DisplayName*>|False|The optional friendly name of the \<xref:System.ServiceModel.Activities.TransactedReceiveScope> activity. The default is TransactedReceiveScope.<br /><br /> Although the \<xref:System.Activities.Activity.DisplayName*> name is not strictly required, it is a best practice to use a display name.|  
|\<xref:System.ServiceModel.Activities.TransactedReceiveScope.Request*>|True|Drops a \<xref:System.ServiceModel.Activities.Receive> activity into the **Request** block on the activity designer surface.|  
|\<xref:System.ServiceModel.Activities.TransactedReceiveScope.Body*>|False|Drops an \<xref:System.Activities.Activity> into the **Body** block on the activity designer surface.|  
  
## See Also  
 [CorrelationScope](../workflowdesigner/correlationscope-activity-designer.md)   
 [InitializeCorrelation](../workflowdesigner/initializecorrelation-activity-designer.md)   
 [Receive](../workflowdesigner/receive-activity-designer.md)   
 [ReceiveAndSendReply](../workflowdesigner/receiveandsendreply-template-designer.md)   
 [Send](../workflowdesigner/send-activity-designer.md)   
 [SendAndReceiveReply](../workflowdesigner/sendandreceivereply-template-designer.md)