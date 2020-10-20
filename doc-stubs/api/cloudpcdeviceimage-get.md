---
title: "Get cloudPcDeviceImage"
description: "Read the properties and relationships of a cloudPcDeviceImage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get cloudPcDeviceImage
Namespace: microsoft.graph

Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdeviceimage"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
    "id": "796e5e56-5e56-796e-565e-6e79565e6e79",
    "displayName": "String",
    "operatingSystem": "String",
    "osBuildNumber": "String",
    "version": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "status": "String",
    "statusDetails": "String",
    "sourceImageResourceId": "String"
  }
}
```
