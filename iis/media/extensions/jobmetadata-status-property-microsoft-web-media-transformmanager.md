﻿---
title: JobMetadata.Status Property  (Microsoft.Web.Media.TransformManager)
TOCTitle: Status Property
ms:assetid: P:Microsoft.Web.Media.TransformManager.JobMetadata.Status
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.transformmanager.jobmetadata.status(v=VS.90)
ms:contentKeyID: 35521097
ms.date: 06/14/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.TransformManager.JobMetadata.Status
- Microsoft.Web.Media.TransformManager.JobMetadata.get_Status
- Microsoft.Web.Media.TransformManager.JobMetadata.set_Status
dev_langs:
- CSharp
- JScript
- VB
- FSharp
- c++
api_location:
- Microsoft.Web.Media.TransformManager.Common.dll
api_name:
- Microsoft.Web.Media.TransformManager.JobMetadata.get_Status
- Microsoft.Web.Media.TransformManager.JobMetadata.set_Status
- Microsoft.Web.Media.TransformManager.JobMetadata.Status
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# Status Property

Gets or sets the status of an ongoing transform.

**Namespace:**  [Microsoft.Web.Media.TransformManager](microsoft-web-media-transformmanager-namespace.md)  
**Assembly:**  Microsoft.Web.Media.TransformManager.Common (in Microsoft.Web.Media.TransformManager.Common.dll)

## Syntax

``` vb
'Declaration
PublicPropertyStatusAsStringGetSet
'Usage
DiminstanceAsJobMetadataDimvalueAsStringvalue = instance.Status

instance.Status = value
```

``` csharp
publicstringStatus { get; set; }
```

``` c++
public:
virtualpropertyString^ Status {
    String^ get () sealed;
    voidset (String^ value) sealed;
}
```

``` fsharp
abstractStatus : stringwithget, setoverrideStatus : stringwithget, set
```

``` jscript
finalfunction getStatus () : Stringfinalfunction setStatus (value : String)
```

#### Property Value

Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
The status.  

#### Implements

[IJobMetadata. . :: . .Status](ijobmetadata-status-property-microsoft-web-media-transformmanager.md)  

## See Also

#### Reference

[JobMetadata Class](jobmetadata-class-microsoft-web-media-transformmanager.md)

[Microsoft.Web.Media.TransformManager Namespace](microsoft-web-media-transformmanager-namespace.md)
