---
title: "fileEncryptionInfo resource type"
description: "Contains properties for file encryption information for the content version of a line of business app."
author: "tfitzmac"
localization_priority: Normal
ms.prod: "intune"
---

# fileEncryptionInfo resource type

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Contains properties for file encryption information for the content version of a line of business app.
## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptionKey|Binary|The key used to encrypt the file content.|
|initializationVector|Binary|The initialization vector used for the encryption algorithm.|
|mac|Binary|The hash of the encrypted file content + IV (content hash).|
|macKey|Binary|The key used to get mac.|
|profileIdentifier|String|The the profile identifier.|
|fileDigest|Binary|The file digest prior to encryption.|
|fileDigestAlgorithm|String|The file digest algorithm.|

## Relationships
None
## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



