# Create share

Use this API to create a new share.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [share](../resources/share.md) object.


### Response
If successful, this method returns `201, Created` response code and [share](../resources/share.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_share_from_serviceprincipals"
}-->
```http
POST /servicePrincipals
```
In the request body, supply a JSON representation of [share](../resources/share.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.share"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 330

{
  "id": "id-value",
  "name": "name-value",
  "owner": {
    "application": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "device": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "user": {
      "displayName": "displayName-value",
      "id": "id-value"
    }
  }
}
```

<!-- uuid: dc544a84-d0b4-4dfa-b55f-0cdebf625db8
2015-10-25 13:21:39 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create share",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->