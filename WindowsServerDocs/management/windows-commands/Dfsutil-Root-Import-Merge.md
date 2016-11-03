---
title: Dfsutil Root Import Merge
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: manage-windows-commands
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: c933843c-38a8-4d95-9716-170b1a2d4a42
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Dfsutil Root Import Merge

>Applies To: Windows Server&reg; 2016, Windows Server&reg; 2012 R2, Windows Server&reg; 2012

The **dfsutil root import merge** command imports folders, folder targets and configuration information for a namespace from a file and merges existing folders and folder targets.



## Syntax

```
dfsutil root import merge <filename> <\\destserver\share> [NoBackup] [Verbose] /?
```

### Parameters

|Parameter|Description|
|-------|--------|
|<\\\\destserver\\share>|UNC path to the namespace to which you want to import the configuration.|
|<filename>|Name of the xml file from which you want to import the namespace configuration.|
|NoBackup|Does not create backup file to restore overwritten folders and folder targets.|
|Verbose|Displays detailed status of the import process.|
|\/?|Displays help at the command prompt.|

## <a name="BKMK_Examples"></a>Examples
To TBD, type:

```
dfsutil root import Merge C:\dir1\docroot.txt \\SRV1\StandaloneNamespace1
```

To enable verbose logging for this command, type:

```
dfsutil root import Merge C:\dir1\docroot.txt \\SRV1\StandaloneNamespace1 /v
```

To view help for this command, type:

```
dfsutil root import Merge /?
```

## Additional references

-   [Command-Line Syntax Key](Command-Line-Syntax-Key.md)

-   [Dfsutil Root](Dfsutil-Root.md)

-   [Dfsutil](Dfsutil.md)

