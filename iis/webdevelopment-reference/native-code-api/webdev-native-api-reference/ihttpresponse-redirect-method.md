---
title: "IHttpResponse::Redirect Method | Microsoft Docs"
ms.custom: ""
ms.date: "10/07/2016"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 1260ee72-2865-b370-00db-11dfde60e0a9
caps.latest.revision: 23
author: "shirhatti"
manager: "wpickett"
---
# IHttpResponse::Redirect Method
Redirects the client to a specified URL.  
  
## Syntax  
  
```cpp  
virtual HRESULT Redirect(  
   IN PCSTR pszUrl,  
   IN BOOL fResetStatusCode = TRUE,  
   IN BOOL fIncludeParameters = FALSE  
) = 0;  
```  
  
#### Parameters  
 `pszUrl`  
 [IN] A pointer to a string that contains the URL for redirection.  
  
 `fResetStatusCode`  
 [IN] `true` to set the HTTP status code to a 302 status; `false` to return an HTML message that indicates the page has been moved.  
  
 `fIncludeParameters`  
 [IN] `true` to pass the query string from the original HTTP request to the redirected URL; otherwise, `false`.  
  
## Return Value  
 An `HRESULT`. Possible values include, but are not limited to, those in the following table.  
  
|Value|Description|  
|-----------|-----------------|  
|S_OK|Indicates that the operation was successful.|  
|ERROR_INVALID_PARAMETER|Indicates that a specified parameter was not valid.|  
|ERROR_NOT_ENOUGH_MEMORY|Indicates that there is insufficient memory to perform the operation.|  
  
## Remarks  
 When the `fResetStatusCode` parameter is `true`, the `Redirect` method automatically redirects a client to a URL specified by the `pszUrl` parameter. When `fResetStatusCode` is `false`, the `Redirect` method returns an HTML message stating that the URL has moved to the new location. If the URL specified by the `pszUrl` parameter is a relative path, the URL will be converted to an absolute URL within the request domain.  
  
> [!NOTE]
>  If you do not return [RQ_NOTIFICATION_FINISH_REQUEST](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/request-notification-status-enumeration.md) from your module after you call the `Redirect` method, the `Redirect` method will not automatically clear the response buffer. In this situation, subsequent processing may add information to the response buffer, and you may receive unexpected results if you do not manually clear the response.  
  
> [!NOTE]
>  The `Redirect` method does not flush the response entity to the client, and any data in the response will be removed when you call the `Redirect` method. If the response has already been flushed to the client, IIS will have sent the existing headers and data to the client, and the `Redirect` method will not redirect the client to the new URL.  
  
## Example  
 The following code example demonstrates how to use the `Redirect` method to create an HTTP module that redirects a client to a relative URL on the Web server.  
  
<!-- TODO: review snippet reference  [!CODE [IHttpResponseRedirect#1](IHttpResponseRedirect#1)]  -->  
  
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
 [IHttpResponse Interface](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/ihttpresponse-interface.md)