﻿---
title: Tracing.ConfigLoaded Property  (Microsoft.Web.Media.Diagnostics)
TOCTitle: ConfigLoaded Property
ms:assetid: P:Microsoft.Web.Media.Diagnostics.Tracing.ConfigLoaded
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.diagnostics.tracing.configloaded(v=VS.90)
ms:contentKeyID: 28440973
ms.date: 05/02/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.Diagnostics.Tracing.ConfigLoaded
- Microsoft.Web.Media.Diagnostics.Tracing.get_ConfigLoaded
dev_langs:
- CSharp
- JScript
- VB
- c++
api_location:
- Microsoft.Web.Media.SmoothStreaming.dll
api_name:
- Microsoft.Web.Media.Diagnostics.Tracing.ConfigLoaded
- Microsoft.Web.Media.Diagnostics.Tracing.get_ConfigLoaded
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# ConfigLoaded Property

Gets the ConfigLoaded property.

**Namespace:**  [Microsoft.Web.Media.Diagnostics](microsoft-web-media-diagnostics-namespace_1.md)  
**Assembly:**  Microsoft.Web.Media.SmoothStreaming (in Microsoft.Web.Media.SmoothStreaming.dll)

## Syntax

``` vb
'Declaration
PublicSharedReadOnlyPropertyConfigLoadedAsBoolean
'Usage
DimvalueAsBooleanvalue = Tracing.ConfigLoaded
```

``` csharp
publicstaticboolConfigLoaded { get; }
```

``` c++
public:
staticpropertyboolConfigLoaded {
    boolget ();
}
```

``` jscript
staticfunction getConfigLoaded () : boolean
```

#### Property Value

Type: [System. . :: . .Boolean](https://msdn.microsoft.com/en-us/library/a28wyd50\(v=vs.90\))  
A Boolean value that specifies whether tracing configuration data has been loaded.  

## Version Information

#### Silverlight

Supported in: 4  

#### Silverlight for Windows Phone

Supported in: Windows Phone OS 7.0  

## Permissions

  - Full trust for the immediate caller. This member cannot be used by partially trusted code. For more information, see [Using Libraries from Partially Trusted Code](https://msdn.microsoft.com/en-us/library/8skskf63\(v=vs.90\)).

## See Also

#### Reference

[Tracing Class](tracing-class-microsoft-web-media-diagnostics_1.md)

[Microsoft.Web.Media.Diagnostics Namespace](microsoft-web-media-diagnostics-namespace_1.md)
