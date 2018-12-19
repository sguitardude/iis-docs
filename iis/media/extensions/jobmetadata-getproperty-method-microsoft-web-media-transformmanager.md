﻿---
title: JobMetadata.GetProperty Method  (Microsoft.Web.Media.TransformManager)
TOCTitle: GetProperty Method
ms:assetid: M:Microsoft.Web.Media.TransformManager.JobMetadata.GetProperty(System.Xml.Linq.XName)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.transformmanager.jobmetadata.getproperty(v=VS.90)
ms:contentKeyID: 35520850
ms.date: 06/14/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.TransformManager.JobMetadata.GetProperty
dev_langs:
- CSharp
- JScript
- VB
- FSharp
- c++
api_location:
- Microsoft.Web.Media.TransformManager.Common.dll
api_name:
- Microsoft.Web.Media.TransformManager.JobMetadata.GetProperty
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# GetProperty Method

Returns the value of the specified property from the task resource description framework (RDF) metadata section in the manifest.

**Namespace:**  [Microsoft.Web.Media.TransformManager](microsoft-web-media-transformmanager-namespace.md)  
**Assembly:**  Microsoft.Web.Media.TransformManager.Common (in Microsoft.Web.Media.TransformManager.Common.dll)

## Syntax

``` vb
'Declaration
PublicFunctionGetProperty ( _
    predicateAsXName _
) AsIManifestProperty
'Usage
DiminstanceAsJobMetadataDimpredicateAsXNameDimreturnValueAsIManifestPropertyreturnValue = instance.GetProperty(predicate)
```

``` csharp
publicIManifestPropertyGetProperty(
    XNamepredicate
)
```

``` c++
public:
virtualIManifestProperty^ GetProperty(
    XName^ predicate
) sealed
```

``` fsharp
abstractGetProperty : 
        predicate:XName->IManifestPropertyoverrideGetProperty : 
        predicate:XName->IManifestProperty
```

``` jscript
publicfinalfunctionGetProperty(
    predicate : XName
) : IManifestProperty
```

#### Parameters

  - predicate  
    Type: [System.Xml.Linq. . :: . .XName](https://msdn.microsoft.com/en-us/library/bb347810\(v=vs.90\))  
    The name of the property to get.  

#### Return Value

Type: [Microsoft.Web.Media.TransformManager. . :: . .IManifestProperty](imanifestproperty-interface-microsoft-web-media-transformmanager.md)  
The property value.  

## See Also

#### Reference

[JobMetadata Class](jobmetadata-class-microsoft-web-media-transformmanager.md)

[Microsoft.Web.Media.TransformManager Namespace](microsoft-web-media-transformmanager-namespace.md)
