﻿---
title: DeploymentAddLinkContext.CreateProvider Method (String, String) (Microsoft.Web.Deployment)
TOCTitle: CreateProvider Method (String, String)
ms:assetid: M:Microsoft.Web.Deployment.DeploymentAddLinkContext.CreateProvider(System.String,System.String)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.deployment.deploymentaddlinkcontext.createprovider(v=VS.90)
ms:contentKeyID: 20209287
ms.date: 05/02/2012
mtps_version: v=VS.90
dev_langs:
- vb
- csharp
- c++
- jscript
api_location:
- Microsoft.Web.Deployment.dll
api_name:
- Microsoft.Web.Deployment.DeploymentAddLinkContext.CreateProvider
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# CreateProvider Method (String, String)

Creates a new deployment object by using the specified provider factory name and path. The new object is added to the underlying collection.

**Namespace:**  [Microsoft.Web.Deployment](microsoft-web-deployment-namespace.md)  
**Assembly:**  Microsoft.Web.Deployment (in Microsoft.Web.Deployment.dll)

## Syntax

``` vb
'Declaration
PublicFunctionCreateProvider ( _
    factoryNameAsString, _
    pathAsString _
) AsDeploymentObjectProvider
'Usage
DiminstanceAsDeploymentAddLinkContextDimfactoryNameAsStringDimpathAsStringDimreturnValueAsDeploymentObjectProviderreturnValue = instance.CreateProvider(factoryName, _
    path)
```

``` csharp
publicDeploymentObjectProviderCreateProvider(
    stringfactoryName,
    stringpath
)
```

``` c++
public:
DeploymentObjectProvider^ CreateProvider(
    String^ factoryName, 
    String^ path
)
```

``` jscript
publicfunctionCreateProvider(
    factoryName : String, 
    path : String
) : DeploymentObjectProvider
```

#### Parameters

  - factoryName  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    The name of the provider factory that is used by the deployment object that this method creates.  

<!-- end list -->

  - path  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    The path of the provider.  

#### Return Value

Type: [Microsoft.Web.Deployment. . :: . .DeploymentObjectProvider](deploymentobjectprovider-class-microsoft-web-deployment.md)  
The [DeploymentObjectProvider](deploymentobjectprovider-class-microsoft-web-deployment.md) object.  

## Remarks

This method creates a deployment object provider that is then used to create a deployment object. This method overload enables the caller to specify the factory name that is used by the deployment provider options and the deployment object provider. After the new deployment object is created, it is added to the deployment object collection of this class.

## Permissions

  - Full trust for the immediate caller. This member cannot be used by partially trusted code. For more information, see [Using Libraries from Partially Trusted Code](https://msdn.microsoft.com/en-us/library/8skskf63\(v=vs.90\)).

## See Also

#### Reference

[DeploymentAddLinkContext Class](deploymentaddlinkcontext-class-microsoft-web-deployment.md)

[CreateProvider Overload](deploymentaddlinkcontext-createprovider-method-microsoft-web-deployment.md)

[Microsoft.Web.Deployment Namespace](microsoft-web-deployment-namespace.md)
