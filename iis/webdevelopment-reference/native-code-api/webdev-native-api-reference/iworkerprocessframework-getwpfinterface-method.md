---
title: "IWorkerProcessFramework::GetWpfInterface Method | Microsoft Docs"
ms.custom: ""
ms.date: "10/07/2016"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 04831e84-27c5-015d-1008-83b0a5ce2966
caps.latest.revision: 22
author: "shirhatti"
manager: "wpickett"
---
# IWorkerProcessFramework::GetWpfInterface Method
Retrieves a defined interface from the worker process framework.  
  
## Syntax  
  
```cpp  
virtual HRESULT GetWpfInterface(  
   IN WPF_INTERFACE_ID_ENUM WpfInterfaceId,  
   OUT PVOID* ppInterface  
) = 0;  
```  
  
#### Parameters  
 `WpfInterfaceId`  
 The ID of the interface to return.  
  
 `ppInterface`  
 A pointer to a buffer that will receive the interface specified by `WpfInterfaceId`.  
  
## Return Value  
 An `HRESULT`. Possible values include, but are not limited to, those in the following table.  
  
|Value|Description|  
|-----------|-----------------|  
|S_OK|Indicates that the operation was successful.|  
  
## Remarks  
 To select which interface to retrieve, choose the specific interface ID from the [WPF_INTERFACE_ID_ENUM](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/wpf-interface-id-enum-enumeration.md) enumeration. If the worker process framework exposes an interface that is not defined by `WPF_INTERFACE_ID_ENUM`, use the [IWorkerProcessFramework::GetCustomInterface](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/iworkerprocessframework-getcustominterface-method.md) method.  
  
## Requirements  
  
|Type|Description|  
|----------|-----------------|  
|Client|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)] on [!INCLUDE[winvista](../../../wmi-provider/includes/winvista-md.md)]<br />-   [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)] on [!INCLUDE[win7](../../../wmi-provider/includes/win7-md.md)]<br />-   [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)] on [!INCLUDE[win8](../../../wmi-provider/includes/win8-md.md)]<br />-   [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)] on [!INCLUDE[win10](../../../wmi-provider/includes/win10-md.md)]|  
|Server|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)] on [!INCLUDE[winsrv2008](../../../wmi-provider/includes/winsrv2008-md.md)]<br />-   [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)] on [!INCLUDE[winsrv2008r2](../../../wmi-provider/includes/winsrv2008r2-md.md)]<br />-   [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)] on [!INCLUDE[winsrv2012](../../../wmi-provider/includes/winsrv2012-md.md)]<br />-   [!INCLUDE[iis85](../../../wmi-provider/includes/iis85-md.md)] on [!INCLUDE[winsrv2012r2](../../../wmi-provider/includes/winsrv2012r2-md.md)]<br />-   [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)] on [!INCLUDE[winsrv2016](../../../wmi-provider/includes/winsrv2016-md.md)]|  
|Product|-   [!INCLUDE[iis70](../../../wmi-provider/includes/iis70-md.md)], [!INCLUDE[iis75](../../../wmi-provider/includes/iis75-md.md)], [!INCLUDE[iis80](../../../wmi-provider/includes/iis80-md.md)], [!INCLUDE[iis85](../../../wmi-provider/includes/iis85-md.md)], [!INCLUDE[iis100](../../../wmi-provider/includes/iis100-md.md)]<br />-   [!INCLUDE[iisexp75](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp75-md.md)], [!INCLUDE[iisexp80](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp80-md.md)], [!INCLUDE[iisexp100](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/includes/iisexp100-md.md)]|  
|Header|Wpframework.h|  
  
## See Also  
 [IWorkerProcessFramework Interface](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/iworkerprocessframework-interface.md)   
 [IWorkerProcessFramework::GetCustomInterface Method](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/iworkerprocessframework-getcustominterface-method.md)   
 [IWorkerProcessFramework::GetInterfaceVersion Method](../../../webdevelopment-reference\native-code-api\webdev-native-api-reference/iworkerprocessframework-getinterfaceversion-method.md)