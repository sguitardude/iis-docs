﻿---
title: Scheduler.GetJobStatus Method  (Microsoft.Web.Media.TransformManager)
TOCTitle: GetJobStatus Method
ms:assetid: M:Microsoft.Web.Media.TransformManager.Scheduler.GetJobStatus(System.String)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.transformmanager.scheduler.getjobstatus(v=VS.90)
ms:contentKeyID: 35521000
ms.date: 06/14/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.TransformManager.Scheduler.GetJobStatus
dev_langs:
- CSharp
- JScript
- VB
- FSharp
- c++
api_location:
- Microsoft.Web.Media.TransformManager.Common.dll
api_name:
- Microsoft.Web.Media.TransformManager.Scheduler.GetJobStatus
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# GetJobStatus Method

Returns the status of the specified job.

**Namespace:**  [Microsoft.Web.Media.TransformManager](microsoft-web-media-transformmanager-namespace.md)  
**Assembly:**  Microsoft.Web.Media.TransformManager.Common (in Microsoft.Web.Media.TransformManager.Common.dll)

## Syntax

``` vb
'Declaration
PublicMustOverrideFunctionGetJobStatus ( _
    jobInstanceIdAsString _
) AsJobStatus
'Usage
DiminstanceAsSchedulerDimjobInstanceIdAsStringDimreturnValueAsJobStatusreturnValue = instance.GetJobStatus(jobInstanceId)
```

``` csharp
publicabstractJobStatusGetJobStatus(
    stringjobInstanceId
)
```

``` c++
public:
virtualJobStatusGetJobStatus(
    String^ jobInstanceId
) abstract
```

``` fsharp
abstractGetJobStatus : 
        jobInstanceId:string->JobStatus
```

``` jscript
publicabstractfunctionGetJobStatus(
    jobInstanceId : String
) : JobStatus
```

#### Parameters

  - jobInstanceId  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    The ID of the job.  

#### Return Value

Type: [Microsoft.Web.Media.TransformManager. . :: . .JobStatus](jobstatus-enumeration-microsoft-web-media-transformmanager.md)  
The status of the job.  

## See Also

#### Reference

[Scheduler Class](scheduler-class-microsoft-web-media-transformmanager.md)

[Microsoft.Web.Media.TransformManager Namespace](microsoft-web-media-transformmanager-namespace.md)
