﻿---
title: TraceEntry Constructor  (Microsoft.Web.Media.Diagnostics)
TOCTitle: TraceEntry Constructor
ms:assetid: M:Microsoft.Web.Media.Diagnostics.TraceEntry.#ctor(System.String,System.String,System.String,Microsoft.Web.Media.Diagnostics.TraceArea,Microsoft.Web.Media.Diagnostics.TraceLevel,System.String)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.web.media.diagnostics.traceentry.traceentry(v=VS.90)
ms:contentKeyID: 23960947
ms.date: 05/02/2012
mtps_version: v=VS.90
f1_keywords:
- Microsoft.Web.Media.Diagnostics.TraceEntry.#ctor
- Microsoft.Web.Media.Diagnostics.TraceEntry.TraceEntry
dev_langs:
- CSharp
- JScript
- VB
- c++
api_location:
- Microsoft.Web.Media.SmoothStreaming.dll
api_name:
- Microsoft.Web.Media.Diagnostics.TraceEntry..ctor
api_type:
- Managed
topic_type:
- apiref
- kbSyntax
product_family_name: VS
ROBOTS: INDEX,FOLLOW
---

# TraceEntry Constructor

Initializes and new instance of the [TraceEntry](traceentry-class-microsoft-web-media-diagnostics_1.md) class.

**Namespace:**  [Microsoft.Web.Media.Diagnostics](microsoft-web-media-diagnostics-namespace_1.md)  
**Assembly:**  Microsoft.Web.Media.SmoothStreaming (in Microsoft.Web.Media.SmoothStreaming.dll)

## Syntax

``` vb
'Declaration
PublicSubNew ( _
    mediaElementIdAsString, _
    classNameAsString, _
    methodNameAsString, _
    traceAreaAsTraceArea, _
    traceLevelAsTraceLevel, _
    textAsString _
)
'Usage
DimmediaElementIdAsStringDimclassNameAsStringDimmethodNameAsStringDimtraceAreaAsTraceAreaDimtraceLevelAsTraceLevelDimtextAsStringDiminstanceAs NewTraceEntry(mediaElementId, _
    className, methodName, traceArea, _
    traceLevel, text)
```

``` csharp
publicTraceEntry(
    stringmediaElementId,
    stringclassName,
    stringmethodName,
    TraceAreatraceArea,
    TraceLeveltraceLevel,
    stringtext
)
```

``` c++
public:
TraceEntry(
    String^ mediaElementId, 
    String^ className, 
    String^ methodName, 
    TraceAreatraceArea, 
    TraceLeveltraceLevel, 
    String^ text
)
```

``` jscript
publicfunctionTraceEntry(
    mediaElementId : String, 
    className : String, 
    methodName : String, 
    traceArea : TraceArea, 
    traceLevel : TraceLevel, 
    text : String
)
```

#### Parameters

  - mediaElementId  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    String value that specifies the media element ID.  

<!-- end list -->

  - className  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    String value that specifies the class name of the method that invoked the trace.  

<!-- end list -->

  - methodName  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    String value that specifies the method name of the method that invoked the trace.  

<!-- end list -->

  - traceArea  
    Type: [Microsoft.Web.Media.Diagnostics. . :: . .TraceArea](tracearea-enumeration-microsoft-web-media-diagnostics_1.md)  
    A [TraceArea](tracearea-enumeration-microsoft-web-media-diagnostics_1.md) enumeration object.  

<!-- end list -->

  - traceLevel  
    Type: [Microsoft.Web.Media.Diagnostics. . :: . .TraceLevel](tracelevel-enumeration-microsoft-web-media-diagnostics_1.md)  
    A [TraceLevel](tracelevel-enumeration-microsoft-web-media-diagnostics_1.md) enumeration object.  

<!-- end list -->

  - text  
    Type: [System. . :: . .String](https://msdn.microsoft.com/en-us/library/s1wwdcbf\(v=vs.90\))  
    String value that specifies the text description of the trace.  

## Version Information

#### Silverlight

Supported in: 4  

#### Silverlight for Windows Phone

Supported in: Windows Phone OS 7.0  

## Permissions

  - Full trust for the immediate caller. This member cannot be used by partially trusted code. For more information, see [Using Libraries from Partially Trusted Code](https://msdn.microsoft.com/en-us/library/8skskf63\(v=vs.90\)).

## See Also

#### Reference

[TraceEntry Class](traceentry-class-microsoft-web-media-diagnostics_1.md)

[Microsoft.Web.Media.Diagnostics Namespace](microsoft-web-media-diagnostics-namespace_1.md)
