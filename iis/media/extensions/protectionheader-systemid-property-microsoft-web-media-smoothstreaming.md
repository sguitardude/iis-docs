﻿---
title: ProtectionHeader.SystemID Property  (Microsoft.Web.Media.SmoothStreaming)
TOCTitle: SystemID Property
ms:assetid: P:Microsoft.Web.Media.SmoothStreaming.ProtectionHeader.SystemID
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.smoothstreaming.protectionheader.systemid(v=VS.90)
ms:contentKeyID: 31469272
ms.date: 05/02/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.SmoothStreaming.ProtectionHeader.get_SystemID
- Microsoft.Web.Media.SmoothStreaming.ProtectionHeader.set_SystemID
- Microsoft.Web.Media.SmoothStreaming.ProtectionHeader.SystemID
dev_langs:
- CSharp
- JScript
- VB
- c++
api_location:
- Microsoft.Web.Media.SmoothStreaming.dll
api_name:
- Microsoft.Web.Media.SmoothStreaming.ProtectionHeader.get_SystemID
- Microsoft.Web.Media.SmoothStreaming.ProtectionHeader.set_SystemID
- Microsoft.Web.Media.SmoothStreaming.ProtectionHeader.SystemID
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# SystemID Property

Gets or sets the GUID that identifies the protection system.

**Namespace:**  [Microsoft.Web.Media.SmoothStreaming](microsoft-web-media-smoothstreaming-namespace_1.md)  
**Assembly:**  Microsoft.Web.Media.SmoothStreaming (in Microsoft.Web.Media.SmoothStreaming.dll)

## Syntax

``` vb
'Declaration
PublicPropertySystemIDAsGuid
'Usage
DiminstanceAsProtectionHeaderDimvalueAsGuidvalue = instance.SystemID
```

``` csharp
publicGuidSystemID { get; internalset; }
```

``` c++
public:
propertyGuidSystemID {
    Guidget ();
    internal: voidset (Guidvalue);
}
```

``` jscript
function getSystemID () : Guidinternalfunction setSystemID (value : Guid)
```

#### Property Value

Type: [System. . :: . .Guid](https://msdn.microsoft.com/en-us/library/cey1zx63\(v=vs.90\))  
A GUID object.  

## Version Information

#### Silverlight

Supported in: 4  

#### Silverlight for Windows Phone

Supported in: Windows Phone OS 7.0  

## Permissions

  - Full trust for the immediate caller. This member cannot be used by partially trusted code. For more information, see [Using Libraries from Partially Trusted Code](https://msdn.microsoft.com/en-us/library/8skskf63\(v=vs.90\)).

## See Also

#### Reference

[ProtectionHeader Class](protectionheader-class-microsoft-web-media-smoothstreaming_1.md)

[Microsoft.Web.Media.SmoothStreaming Namespace](microsoft-web-media-smoothstreaming-namespace_1.md)
