﻿---
title: DeploymentManager.ProviderFactories Property  (Microsoft.Web.Deployment)
TOCTitle: ProviderFactories Property
ms:assetid: P:Microsoft.Web.Deployment.DeploymentManager.ProviderFactories
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.deployment.deploymentmanager.providerfactories(v=VS.90)
ms:contentKeyID: 20208649
ms.date: 05/02/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Deployment.DeploymentManager.ProviderFactories
- Microsoft.Web.Deployment.DeploymentManager.get_ProviderFactories
dev_langs:
- CSharp
- JScript
- VB
- c++
api_location:
- Microsoft.Web.Deployment.dll
api_name:
- Microsoft.Web.Deployment.DeploymentManager.get_ProviderFactories
- Microsoft.Web.Deployment.DeploymentManager.ProviderFactories
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# ProviderFactories Property

**Namespace:**  [Microsoft.Web.Deployment](microsoft-web-deployment-namespace.md)  
**Assembly:**  Microsoft.Web.Deployment (in Microsoft.Web.Deployment.dll)

## Syntax

``` vb
'Declaration
PublicSharedReadOnlyPropertyProviderFactoriesAsIEnumerable(OfDeploymentProviderFactory)
'Usage
DimvalueAsIEnumerable(OfDeploymentProviderFactory)

value = DeploymentManager.ProviderFactories
```

``` csharp
publicstaticIEnumerable<DeploymentProviderFactory> ProviderFactories { get; }
```

``` c++
public:
staticpropertyIEnumerable<DeploymentProviderFactory^>^ ProviderFactories {
    IEnumerable<DeploymentProviderFactory^>^ get ();
}
```

``` jscript
staticfunction getProviderFactories () : IEnumerable<DeploymentProviderFactory>
```

#### Property Value

Type: [System.Collections.Generic. . :: . .IEnumerable](https://msdn.microsoft.com/en-us/library/9eekhta0\(v=vs.90\))\< (Of \< ( \<'[DeploymentProviderFactory](deploymentproviderfactory-class-microsoft-web-deployment.md)\> ) \> ) \>  
Returns [IEnumerable\<(Of \<(\<'T\>)\>)\>](https://msdn.microsoft.com/en-us/library/9eekhta0\(v=vs.90\)).  

## Permissions

  - Full trust for the immediate caller. This member cannot be used by partially trusted code. For more information, see [Using Libraries from Partially Trusted Code](https://msdn.microsoft.com/en-us/library/8skskf63\(v=vs.90\)).

## See Also

#### Reference

[DeploymentManager Class](deploymentmanager-class-microsoft-web-deployment.md)

[Microsoft.Web.Deployment Namespace](microsoft-web-deployment-namespace.md)
