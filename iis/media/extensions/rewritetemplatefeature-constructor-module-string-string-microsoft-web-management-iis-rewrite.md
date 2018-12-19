﻿---
title: RewriteTemplateFeature Constructor (Module, String, String) (Microsoft.Web.Management.Iis.Rewrite)
TOCTitle: RewriteTemplateFeature Constructor (Module, String, String)
ms:assetid: M:Microsoft.Web.Management.Iis.Rewrite.RewriteTemplateFeature.#ctor(Microsoft.Web.Management.Client.Module,System.String,System.String)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.management.iis.rewrite.rewritetemplatefeature.rewritetemplatefeature(v=VS.90)
ms:contentKeyID: 20476358
ms.date: 05/02/2012
mtps_version: v=VS.90
dev_langs:
- vb
- csharp
- c++
- jscript
api_location:
- Microsoft.Web.Management.Rewrite.Client.dll
api_name:
- Microsoft.Web.Management.Iis.Rewrite.RewriteTemplateFeature..ctor
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# RewriteTemplateFeature Constructor (Module, String, String)

Creates an instance of a [RewriteTemplateFeature](rewritetemplatefeature-class-microsoft-web-management-iis-rewrite.md) object with the given module, title, and description.

**Namespace:**  [Microsoft.Web.Management.Iis.Rewrite](microsoft-web-management-iis-rewrite-namespace.md)  
**Assembly:**  Microsoft.Web.Management.Rewrite.Client (in Microsoft.Web.Management.Rewrite.Client.dll)

## Syntax

``` vb
'Declaration
ProtectedSubNew ( _
    moduleAsModule, _
    titleAsString, _
    descriptionAsString _
)
'Usage
DimmoduleAs [Module]
DimtitleAsStringDimdescriptionAsStringDiminstanceAs NewRewriteTemplateFeature(module, _
    title, description)
```

``` csharp
protectedRewriteTemplateFeature(
    Modulemodule,
    stringtitle,
    stringdescription
)
```

``` c++
protected:
RewriteTemplateFeature(
    Module^ module, 
    String^ title, 
    String^ description
)
```

``` jscript
protectedfunctionRewriteTemplateFeature(
    module : Module, 
    title : String, 
    description : String
)
```

#### Parameters

  - module  
    Type: [Microsoft.Web.Management.Client. . :: . .Module](https://msdn.microsoft.com/en-us/library/ms634308\(v=vs.90\))  
    The client-side user interface module for this feature.  

<!-- end list -->

  - title  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    The title displayed on the client-side user interface for this feature.  

<!-- end list -->

  - description  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    The description displayed on the client-side user interface for this feature.  

## Exceptions

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Exception</th>
<th>Condition</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>[ArgumentNullException]</td>
<td><p>The module, title or description parameters are null Nothing nullptr unit a null reference (Nothing in Visual Basic) (Nothing in Visual Basic).</p></td>
</tr>
</tbody>
</table>


## Permissions

  - Full trust for the immediate caller. This member cannot be used by partially trusted code. For more information, see [Using Libraries from Partially Trusted Code](https://msdn.microsoft.com/en-us/library/8skskf63\(v=vs.90\)).

## See Also

#### Reference

[RewriteTemplateFeature Class](rewritetemplatefeature-class-microsoft-web-management-iis-rewrite.md)

[RewriteTemplateFeature Overload](rewritetemplatefeature-constructor-microsoft-web-management-iis-rewrite.md)

[Microsoft.Web.Management.Iis.Rewrite Namespace](microsoft-web-management-iis-rewrite-namespace.md)
