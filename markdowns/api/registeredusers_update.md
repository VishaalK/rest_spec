# Update the properties of registeredusers object.

Update the properties of registeredusers object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/<objectId>
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|accountEnabled|Boolean||
|alternativeSecurityIds|AlternativeSecurityId||
|approximateLastLogonTimestamp|DateTimeOffset||
|deletionTimestamp|DateTimeOffset||
|deviceId|Guid||
|deviceMetadata|String||
|deviceOSType|String||
|deviceOSVersion|String||
|deviceObjectVersion|Int32||
|devicePhysicalIds|String||
|deviceTrustType|String||
|dirSyncEnabled|Boolean||
|displayName|String||
|lastDirSyncTime|DateTimeOffset||
|objectType|String||

### Response
If successful, this method returns a `200 OK` response code and updated [registeredUsers](../resources/registeredusers.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_registeredusers"
}-->
```http
PUT /devices/<objectId>
Content-type: application/json
Content-length: 3

{
}
```
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.registeredusers"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: dc544a84-d0b4-4dfa-b55f-0cdebf625db8
2015-10-25 13:21:39 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update the properties of registeredusers object.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->