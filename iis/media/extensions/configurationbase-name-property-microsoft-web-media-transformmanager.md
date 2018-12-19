﻿---
title: ConfigurationBase.Name Property  (Microsoft.Web.Media.TransformManager)
TOCTitle: Name Property
ms:assetid: P:Microsoft.Web.Media.TransformManager.ConfigurationBase.Name
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.transformmanager.configurationbase.name(v=VS.90)
ms:contentKeyID: 35520942
ms.date: 06/14/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.TransformManager.ConfigurationBase.Name
- Microsoft.Web.Media.TransformManager.ConfigurationBase.get_Name
- Microsoft.Web.Media.TransformManager.ConfigurationBase.set_Name
dev_langs:
- CSharp
- JScript
- VB
- FSharp
- c++
api_location:
- Microsoft.Web.Media.TransformManager.Common.dll
api_name:
- Microsoft.Web.Media.TransformManager.ConfigurationBase.get_Name
- Microsoft.Web.Media.TransformManager.ConfigurationBase.Name
- Microsoft.Web.Media.TransformManager.ConfigurationBase.set_Name
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# Name Property

Gets or sets the XML element name of the IIS Transform Manager configuration.

**Namespace:**  [Microsoft.Web.Media.TransformManager](microsoft-web-media-transformmanager-namespace.md)  
**Assembly:**  Microsoft.Web.Media.TransformManager.Common (in Microsoft.Web.Media.TransformManager.Common.dll)

## Syntax

``` vb
'Declaration
<DataMemberAttribute> _
PublicPropertyNameAsStringGetSet
'Usage
DiminstanceAsConfigurationBaseDimvalueAsStringvalue = instance.Name

instance.Name = value
```

``` csharp
[DataMemberAttribute]
publicstringName { get; set; }
```

``` c++
[DataMemberAttribute]
public:
propertyString^ Name {
    String^ get ();
    voidset (String^ value);
}
```

``` fsharp
[<DataMemberAttribute>]
memberName : stringwithget, set
```

``` jscript
function getName () : Stringfunction setName (value : String)
```

#### Property Value

Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
The name of the XML element.  

## Remarks

This property is a string value that is the name of the configuration object that this object is the base of. The base class exposes properties and a corresponding XElement object that is useful for creating the XML representation for persistence.

## See Also

#### Reference

[ConfigurationBase Class](configurationbase-class-microsoft-web-media-transformmanager.md)

[Microsoft.Web.Media.TransformManager Namespace](microsoft-web-media-transformmanager-namespace.md)
