﻿---
title: AdaptiveSourceManagerFailedEventHandler Delegate
TOCTitle: AdaptiveSourceManagerFailedEventHandler Delegate
ms:assetid: 16ef48ff-cdfc-445d-8f84-cdc52cc5f575
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ822683(v=VS.90)
ms:contentKeyID: 50079438
ms.date: 11/19/2012
mtps_version: v=VS.90
dev_langs:
- csharp
- c++
---

# AdaptiveSourceManagerFailedEventHandler Delegate

**Applies to:** Windows Store apps only

The actual handler for the adaptive source manager failed event handler.

## Syntax

``` csharp
[GuidAttribute(, , , , , , , , , , )]
[VersionAttribute()]
public delegate void AdaptiveSourceManagerFailedEventHandler(
AdaptiveSourceManager sender,
AdaptiveSourceManagerFailedEventArgs args
)
```

``` c++
[GuidAttribute(, , , , , , , , , , )]
[VersionAttribute()]
public delegate void AdaptiveSourceManagerFailedEventHandler(
[InAttribute] AdaptiveSourceManager^ sender, 
[InAttribute] AdaptiveSourceManagerFailedEventArgs^ args
)
```

## Parameters

  - sender  
    Adaptive source manager this event belongs to

  - AdaptiveSourceManagerFailedEventArgs  
    Event arguments

## Return Value

If the method succeeds, it returns S\_OK. Otherwise, it returns an HRESULT error code.

## Requirements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Minimum supported client</strong></p></td>
<td><p>Windows 8</p></td>
</tr>
<tr class="even">
<td><p><strong>Minimum supported server</strong></p></td>
<td><p>Not Supported</p></td>
</tr>
<tr class="odd">
<td><p><strong>Metadata</strong></p></td>
<td><p>Microsoft.Media.AdaptiveStreaming.winmd</p></td>
</tr>
</tbody>
</table>
