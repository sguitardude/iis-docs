﻿---
title: TransformManagerService.GetCumulativeJobCountByStatus Method  (Microsoft.Web.Media.TransformManager)
TOCTitle: GetCumulativeJobCountByStatus Method
ms:assetid: M:Microsoft.Web.Media.TransformManager.TransformManagerService.GetCumulativeJobCountByStatus(Microsoft.Web.Media.TransformManager.JobStatus)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.transformmanager.transformmanagerservice.getcumulativejobcountbystatus(v=VS.90)
ms:contentKeyID: 46408636
ms.date: 06/14/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.TransformManager.TransformManagerService.GetCumulativeJobCountByStatus
dev_langs:
- CSharp
- JScript
- VB
- FSharp
- c++
api_location:
- Microsoft.Web.Media.TransformManager.ServiceLibrary.dll
api_name:
- Microsoft.Web.Media.TransformManager.TransformManagerService.GetCumulativeJobCountByStatus
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# GetCumulativeJobCountByStatus Method

**Namespace:**  [Microsoft.Web.Media.TransformManager](microsoft-web-media-transformmanager-namespace.md)  
**Assembly:**  Microsoft.Web.Media.TransformManager.ServiceLibrary (in Microsoft.Web.Media.TransformManager.ServiceLibrary.dll)

## Syntax

``` vb
'Declaration
<PrincipalPermissionAttribute(SecurityAction.Demand, Role := "Administrators")> _
PublicFunctionGetCumulativeJobCountByStatus ( _
    statusAsJobStatus _
) AsInteger
'Usage
DiminstanceAsTransformManagerServiceDimstatusAsJobStatusDimreturnValueAsIntegerreturnValue = instance.GetCumulativeJobCountByStatus(status)
```

``` csharp
[PrincipalPermissionAttribute(SecurityAction.Demand, Role = "Administrators")]
publicintGetCumulativeJobCountByStatus(
    JobStatusstatus
)
```

``` c++
[PrincipalPermissionAttribute(SecurityAction::Demand, Role = L"Administrators")]
public:
virtualintGetCumulativeJobCountByStatus(
    JobStatusstatus
) sealed
```

``` fsharp
[<PrincipalPermissionAttribute(SecurityAction.Demand, Role = "Administrators")>]
abstractGetCumulativeJobCountByStatus : 
        status:JobStatus->int 
[<PrincipalPermissionAttribute(SecurityAction.Demand, Role = "Administrators")>]
overrideGetCumulativeJobCountByStatus : 
        status:JobStatus->int
```

``` jscript
publicfinalfunctionGetCumulativeJobCountByStatus(
    status : JobStatus
) : int
```

#### Parameters

  - status  
    Type: [Microsoft.Web.Media.TransformManager. . :: . .JobStatus](jobstatus-enumeration-microsoft-web-media-transformmanager.md)  

#### Return Value

Type: [System. . :: . .Int32](https://msdn.microsoft.com/en-us/library/td2s409d\(v=vs.90\))  

#### Implements

[IMonitoringService. . :: . .GetCumulativeJobCountByStatus(JobStatus)](imonitoringservice-getcumulativejobcountbystatus-method-microsoft-web-media-transformmanager.md)  

## See Also

#### Reference

[TransformManagerService Class](transformmanagerservice-class-microsoft-web-media-transformmanager.md)

[Microsoft.Web.Media.TransformManager Namespace](microsoft-web-media-transformmanager-namespace.md)
