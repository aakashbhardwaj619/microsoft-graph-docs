---
title: "Create linkedResource"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create linkedResource

Namespace: microsoft.graph

Create a new linkedResource object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request Body

In the request body, supply JSON representation of the [linkedResource](../resources/-linkedresource.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a linkedResource object.

| Property        | Type   | Description |
| :-------------- | :----- | :---------- |
| applicationName | String |             |
| displayName     | String |             |
| externalId      | String |             |
| id              | String | Read-only.  |
| webUrl          | String |             |

## Response

If successful, this method returns a `201 Created` response code and a linkedResource object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_linkedresource"
}
-->

```http
POST https://graph.microsoft.com/v1.0

Content-Type: application/json
Content-Length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String",
  "webUrl": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.toDo.linkedResource"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.linkedResource",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String(identifier)",
  "webUrl": "String"
}
}

```