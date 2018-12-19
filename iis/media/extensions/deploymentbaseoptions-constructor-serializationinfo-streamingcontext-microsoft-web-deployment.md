﻿---
title: DeploymentBaseOptions Constructor (SerializationInfo, StreamingContext) (Microsoft.Web.Deployment)
TOCTitle: DeploymentBaseOptions Constructor (SerializationInfo, StreamingContext)
ms:assetid: M:Microsoft.Web.Deployment.DeploymentBaseOptions.#ctor(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.deployment.deploymentbaseoptions.deploymentbaseoptions(v=VS.90)
ms:contentKeyID: 20209089
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
- Microsoft.Web.Deployment.DeploymentBaseOptions..ctor
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# DeploymentBaseOptions Constructor (SerializationInfo, StreamingContext)

**Namespace:**  [Microsoft.Web.Deployment](microsoft-web-deployment-namespace.md)  
**Assembly:**  Microsoft.Web.Deployment (in Microsoft.Web.Deployment.dll)

## Syntax

``` vb
'Declaration
ProtectedSubNew ( _
    infoAsSerializationInfo, _
    contextAsStreamingContext _
)
'Usage
DiminfoAsSerializationInfoDimcontextAsStreamingContextDiminstanceAs NewDeploymentBaseOptions(info, context)
```

``` csharp
protectedDeploymentBaseOptions(
    SerializationInfoinfo,
    StreamingContextcontext
)
```

``` c++
protected:
DeploymentBaseOptions(
    SerializationInfo^ info, 
    StreamingContextcontext
)
```

``` jscript
protectedfunctionDeploymentBaseOptions(
    info : SerializationInfo, 
    context : StreamingContext
)
```

#### Parameters

  - info  
    Type: [System.Runtime.Serialization. . :: . .SerializationInfo](https://msdn.microsoft.com/en-us/library/a9b6042e\(v=vs.90\))  

<!-- end list -->

  - context  
    Type: [System.Runtime.Serialization. . :: . .StreamingContext](https://msdn.microsoft.com/en-us/library/t16abws5\(v=vs.90\))  

## Permissions

  - Full trust for the immediate caller. This member cannot be used by partially trusted code. For more information, see [Using Libraries from Partially Trusted Code](https://msdn.microsoft.com/en-us/library/8skskf63\(v=vs.90\)).

## See Also

#### Reference

[DeploymentBaseOptions Class](deploymentbaseoptions-class-microsoft-web-deployment.md)

[DeploymentBaseOptions Overload](deploymentbaseoptions-constructor-microsoft-web-deployment.md)

[Microsoft.Web.Deployment Namespace](microsoft-web-deployment-namespace.md)
