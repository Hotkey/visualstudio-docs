---
title: "API Reference for Testing Tools for Visual Studio ALM"
ms.custom: na
ms.date: 10/03/2016
ms.prod: visual-studio-tfs-dev14
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 5c55f1a9-3f08-4244-8c91-1e912e69e8d2
caps.latest.revision: 22
manager: douge
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
# API Reference for Testing Tools for Visual Studio ALM
Use this API reference to help you extend existing features or add new capabilities. For example, you can create different kinds of tests. For sample code that shows how you might use these APIs, see this [Microsoft Web site](http://go.microsoft.com/fwlink/?LinkId=185591).  
  
 **Requirements**  
  
-   Visual Studio Enterprise  
  
## Tasks  
  
|Tasks|Associated Topics|  
|-----------|-----------------------|  
|**Extend the unit test framework:** You can add functionality to your tests that might not be in the Unit Test Framework. For example, you can add a test property that specifies if a test should run as a normal user or not. Or you can extend the framework to add row attributes to a method and use the data in that row inside the test.|-   <xref:Microsoft.VisualStudio.TestTools.Common?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.Vsip?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.UnitTesting?qualifyHint=False><br /><br /> For sample code of how to extend the unit test framework, see the following [Microsoft Web site](http://go.microsoft.com/fwlink/?LinkId=185591).|  
|**Customize test storage processes:** The <xref:Microsoft.VisualStudio.TestTools.Common.Xml?qualifyHint=False> namespace provides an interface that you can use for loading and storing tests. You can implement these as you create your own test types.|-   <xref:Microsoft.VisualStudio.TestTools.Common.Xml?qualifyHint=False>|  
|**Create a custom exception:** You can create custom exception that can be thrown by the Unit Testing framework.|-   <xref:Microsoft.VisualStudio.TestTools.Exceptions?qualifyHint=False>|  
|**Create a Diagnostic Data Adapter:** You can use the <xref:Microsoft.VisualStudio.TestTools.Execution?qualifyHint=False> to create a custom Diagnostic Data Adapter.|-   <xref:Microsoft.VisualStudio.TestTools.Execution?qualifyHint=False><br />-   [Creating a Diagnostic Data Adapter to Collect Custom Data or Affect a Test Machine](../dv_TeamTestALM/Creating-a-Diagnostic-Data-Adapter-to-Collect-Custom-Data-or-Affect-a-Test-Machine.md)<br />-   [Sample Project for Creating a Diagnostic Data Adapter](../dv_TeamTestALM/Sample-Project-for-Creating-a-Diagnostic-Data-Adapter.md)|  
|**Create load tests for unit and Web tests:** The <xref:Microsoft.VisualStudio.TestTools.LoadTesting?qualifyHint=False> namespace provides classes and interfaces that enable you to extend load testing of unit and Web tests.|-   <xref:Microsoft.VisualStudio.TestTools.LoadTesting?qualifyHint=False>|  
|**Create a test type:** Use the <xref:Microsoft.VisualStudio.TestTools.TestAdapter?qualifyHint=False> framework and the <xref:Microsoft.VisualStudio.TestTools.Vsip?qualifyHint=False> to create your own test type.|-   <xref:Microsoft.VisualStudio.TestTools.TestAdapter?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.Vsip?qualifyHint=False><br />-   [Customizing for Testing By Using the Visual Studio SDK](assetId:///9cf7a840-dd66-4b00-90f7-e00e40370a69)|  
|**Creating coded UI tests to automate your user interface:** The <xref:Microsoft.VisualStudio.TestTools.UITesting?qualifyHint=False> namespace supplies classes that provide coded UI test support. This namespace contains classes to perform keyboard and mouse interactions on user interface controls.<br /><br /> You can also derive from classes in the <xref:Microsoft.VisualStudio.TestTools.UITest.Extension?qualifyHint=False> namespace to extend the coded UI testing capability to record tests on currently unsupported interfaces, such as Microsoft Excel.|-   [Use UI Automation To Test Your Code](../VS_IDE/Use-UI-Automation-To-Test-Your-Code.md)<br />-   [Extending Coded UI Tests and Action Recordings to Support Microsoft Excel](../VS_IDE/Extending-Coded-UI-Tests-and-Action-Recordings-to-Support-Microsoft-Excel.md)<br />-   <xref:Microsoft.VisualStudio.TestTools.UITesting?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.UITesting.HtmlControls?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.UITesting.WinControls?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.UITesting.WpfControls?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.UITest.Common?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.UITest.Common.UIMap?qualifyHint=False><br />-   <xref:Microsoft.VisualStudio.TestTools.UITest.Extension?qualifyHint=False>|  
|**Creating Unit Tests to Verify the Quality of Your Code:** The <xref:Microsoft.VisualStudio.TestTools.UnitTesting?qualifyHint=False> namespace has classes that provide unit testing support. This namespace contains many attributes that identify test information to the testing framework regarding data sources, order of method execution, program management, agent/host information, and deployment data. This namespace also contains custom unit testing exceptions.|-   <xref:Microsoft.VisualStudio.TestTools.UnitTesting?qualifyHint=False><br />-   [Unit Test Your Code](../VS_IDE/Unit-Test-Your-Code.md)|  
|**Create Unit Tests for ASP.NET and Web Services:** The <xref:Microsoft.VisualStudio.TestTools.UnitTesting.Web?qualifyHint=False> namespace is an extension of the <xref:Microsoft.VisualStudio.TestTools.UnitTesting?qualifyHint=False> namespace that provides ASP.NET and Web service unit test capabilities. This namespace provides a set of attributes to unit tests that define credentials, URLs, and server specific information.|-   <xref:Microsoft.VisualStudio.TestTools.UnitTesting.Web?qualifyHint=False><br />-   [Unit Test Your Code](../VS_IDE/Unit-Test-Your-Code.md)|  
|**Create Custom Web Tests:** The classes in the <xref:Microsoft.VisualStudio.TestTools.WebTesting?qualifyHint=False> namespace enable Web testing. Additionally, it includes classes for data binding, test rules, identifying work items, query strings, HTTP context, and plug-ins that provide testing features.|-   <xref:Microsoft.VisualStudio.TestTools.WebTesting?qualifyHint=False>|  
|**Customize Web Tests Using Rules:** The <xref:Microsoft.VisualStudio.TestTools.WebTesting.Rules?qualifyHint=False> namespace contains a set of rules used by Web tests to test Web pages. These rules provide a set of tools for Web tests to test the content of Web pages. Additionally, custom rules can be created to extend the functionality of Web tests.|-   <xref:Microsoft.VisualStudio.TestTools.WebTesting.Rules?qualifyHint=False>|  
  
## See Also  
 [Test apps early and often](../dv_TeamTestALM/Test-apps-early-and-often.md)   
 [Creating a Diagnostic Data Adapter to Collect Custom Data or Affect a Test Machine](../dv_TeamTestALM/Creating-a-Diagnostic-Data-Adapter-to-Collect-Custom-Data-or-Affect-a-Test-Machine.md)   
 [Use UI Automation To Test Your Code](../VS_IDE/Use-UI-Automation-To-Test-Your-Code.md)   
 [Extending Coded UI Tests and Action Recordings to Support Microsoft Excel](../VS_IDE/Extending-Coded-UI-Tests-and-Action-Recordings-to-Support-Microsoft-Excel.md)   
 [Unit Test Your Code](../VS_IDE/Unit-Test-Your-Code.md)