---
title: "IHttpServer::GetTraceContext Method | Microsoft Docs"
ms.custom: ""
ms.date: "10/07/2016"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: f1f6b14a-e7a6-948f-89f4-cdebea2b8a87
caps.latest.revision: 10
author: "shirhatti"
manager: "wpickett"
---
# IHttpServer::GetTraceContext Method
Retrieves an [IHttpTraceContext](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/ihttptracecontext-interface.md) interface.  
  
## Syntax  
  
```cpp  
virtual IHttpTraceContext* GetTraceContext(  
   VOID  
) const = 0;  
```  
  
#### Parameters  
 This method takes no parameters.  
  
## Return Value  
 A pointer to an `IHttpTraceContext` interface.  
  
## Remarks  
 Use the `IHttpServer::GetTraceContext` method to retrieve an `IHttpTraceContext` interface when you need to raise an event that is not associated with an HTTP request. When you need to raise an event that is associated with an HTTP request, use either the `IHttpServer::GetTraceContext` or [IHttpContext::GetTraceContext](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/ihttpcontext-gettracecontext-method.md) method to retrieve an `IHttpTraceContext` interface.  
  
## Example  
 The following code example demonstrates how to create an HTTP module that performs the following tasks:  
  
1.  Retrieves a pointer to an `IHttpTraceContext` interface by using the `IHttpServer::GetTraceContext` method.  
  
2.  Retrieves the trace activity GUID by using the [IHttpTraceContext::GetTraceActivityId](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/ihttptracecontext-gettraceactivityid-method.md) method.  
  
3.  Creates a string that contains the trace activity GUID and writes the string to the Event Viewer.  
  
<!-- TODO: review snippet reference  [!CODE [IHttpServerGetTraceContext#1](IHttpServerGetTraceContext#1)]  -->  
  
 Your module must export the [RegisterModule](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/pfn-registermodule-function.md) function. You can export this function by creating a module definition (.def) file for your project, or you can compile the module by using the `/EXPORT:RegisterModule` switch. For more information, see [Walkthrough: Creating a Request-Level HTTP Module By Using Native Code](../../../webdevelopment-reference\native-code-development-overview\native-code-dev-overview/walkthrough-creating-a-request-level-http-module-by-using-native-code.md).  
  
 You can optionally compile the code by using the `__stdcall (/Gz)` calling convention instead of explicitly declaring the calling convention for each function.  
  
## Requirements  
  
|Type|Description|  
|----------|-----------------|  
|Client|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)] on [!INCLUDE[winvista](../../../wmi-provider/includes/winvista-md.md)]<br />-   [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)] on [!INCLUDE[win7](../../../wmi-provider/includes/win7-md.md)]<br />-   [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)] on [!INCLUDE[win8](../../../wmi-provider/includes/win8-md.md)]<br />-   [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)] on [!INCLUDE[win10](../../../wmi-provider/includes/win10-md.md)]|  
|Server|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)] on [!INCLUDE[winsrv2008](../../../wmi-provider/includes/winsrv2008-md.md)]<br />-   [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)] on [!INCLUDE[winsrv2008r2](../../../wmi-provider/includes/winsrv2008r2-md.md)]<br />-   [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)] on [!INCLUDE[winsrv2012](../../../wmi-provider/includes/winsrv2012-md.md)]<br />-   [!INCLUDE[iis85](../../../wmi-provider/includes/iis85-md.md)] on [!INCLUDE[winsrv2012r2](../../../wmi-provider/includes/winsrv2012r2-md.md)]<br />-   [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)] on [!INCLUDE[winsrv2016](../../../wmi-provider/includes/winsrv2016-md.md)]|  
|Product|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)], [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)], [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)], [!INCLUDE[iis85](../../../wmi-provider/includes/iis85-md.md)], [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)]<br />-   [!INCLUDE[iisexp75](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp75-md.md)], [!INCLUDE[iisexp80](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp80-md.md)], [!INCLUDE[iisexp100](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp100-md.md)]|  
|Header|Httpserv.h|  
  
## See Also  
 [IHttpServer Interface](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/ihttpserver-interface.md)   
 [IHttpContext::GetTraceContext Method](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/ihttpcontext-gettracecontext-method.md)   
 [IHttpTraceContext Interface](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/ihttptracecontext-interface.md)