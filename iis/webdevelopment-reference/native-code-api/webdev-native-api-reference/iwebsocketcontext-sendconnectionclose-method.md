---
title: "IWebSocketContext::SendConnectionClose Method | Microsoft Docs"
ms.custom: ""
ms.date: "10/07/2016"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: e2870934-24f9-4e42-a9eb-affe437eccc6
caps.latest.revision: 5
author: "shirhatti"
manager: "wpickett"
---
# IWebSocketContext::SendConnectionClose Method
Signals the close of a WebSocket connection.  
  
## Syntax  
  
```cpp  
virtual HRESULT SendConnectionClose(  
   _In_ BOOL fAsync,  
   _In_ USHORT* pStatusCode = NULL,  
   _In_ LPCWSTR pszReason = NULL,  
   _In_ PFN_WEBSOCKET_COMPLETION pfnCompletion = NULL,  
   _In_ VOID* pvCompletionContext = NULL,  
   _Out_ BOOL* pfCompletionExpected = NULL  
) = 0;  
```  
  
#### Parameters  
 `fAsync`  
 [IN] `true` if the method should complete asynchronously; otherwise, `false`.  
  
 `pStatusCode`  
 [IN] Points to the status code for the connection.  
  
 `pszReason`  
 [IN] Points to the reason text for the status.  
  
 `pfnCompletion`  
 [IN] Points to the function that will complete the operation.  
  
 `pvCompletionContext`  
 [IN] Points to the completion context information for the operation.  
  
 `pfCompletionExpected`  
 [OUT] `true` if an asynchronous completion is pending for this call; otherwise, `false`.  
  
## Return Value  
 An `HRESULT`. Possible values include, but are not limited to, those in the following table.  
  
|Value|Description|  
|-----------|-----------------|  
|S_OK|Indicates that the operation was successful.|  
  
## Requirements  
  
|Type|Description|  
|----------|-----------------|  
|Client|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)] on [!INCLUDE[winvista](../../../wmi-provider/includes/winvista-md.md)]<br />-   [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)] on [!INCLUDE[win7](../../../wmi-provider/includes/win7-md.md)]<br />-   [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)] on [!INCLUDE[win8](../../../wmi-provider/includes/win8-md.md)]<br />-   [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)] on [!INCLUDE[win10](../../../wmi-provider/includes/win10-md.md)]|  
|Server|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)] on [!INCLUDE[winsrv2008](../../../wmi-provider/includes/winsrv2008-md.md)]<br />-   [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)] on [!INCLUDE[winsrv2008r2](../../../wmi-provider/includes/winsrv2008r2-md.md)]<br />-   [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)] on [!INCLUDE[winsrv2012](../../../wmi-provider/includes/winsrv2012-md.md)]<br />-   [!INCLUDE[iis85](../../../wmi-provider/includes/iis85-md.md)] on [!INCLUDE[winsrv2012r2](../../../wmi-provider/includes/winsrv2012r2-md.md)]<br />-   [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)] on [!INCLUDE[winsrv2016](../../../wmi-provider/includes/winsrv2016-md.md)]|  
|Product|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)], [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)], [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)], [!INCLUDE[iis85](../../../wmi-provider/includes/iis85-md.md)], [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)]<br />-   [!INCLUDE[iisexp75](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp75-md.md)], [!INCLUDE[iisexp80](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp80-md.md)], [!INCLUDE[iisexp100](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp100-md.md)]|  
|Header|Iiswebsocket.h|  
  
## See Also  
 [IWebSocketContext Interface](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/iwebsocketcontext-interface.md)