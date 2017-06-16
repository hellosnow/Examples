## Request

```http
POST https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res7439/providers/Microsoft.Storage/storageAccounts/sto1299/ListServiceSas?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Length: 137
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: 85228de5-1398-48f2-918b-fc67fc9ed92e
host: management.azure.com
Connection: close

{"canonicalizedResource":"/blob/sto1299/music","signedResource":"c","signedPermission":"l","signedExpiry":"2017-05-24T11:32:48.8457197Z"}
```

## Curl

```bash
curl -X POST 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res7439/providers/Microsoft.Storage/storageAccounts/sto1299/ListServiceSas?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \ 
-H 'Content-Length: 137' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: 85228de5-1398-48f2-918b-fc67fc9ed92e' \
-d { \
  "canonicalizedResource": "/blob/sto1299/music", \
  "signedResource": "c", \
  "signedPermission": "l", \
  "signedExpiry": "2017-05-24T11:32:48.8457197Z" \
}
```

## Response

#### StatusCode: 200

```http
HTTP 1.1 200
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: 0d9c9634-21e1-47e2-891c-e777de6853c2
x-ms-correlation-request-id: 0d9c9634-21e1-47e2-891c-e777de6853c2
x-ms-routing-request-id: WESTUS2:20170615T095442420Z:0d9c9634-21e1-47e2-891c-e777de6853c2
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 124
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"serviceSasToken":"sv=2015-04-05&sr=c&se=2017-05-24T11%3A32%3A48Z&sp=l&sig=PoF8yBUGixsjzwroLmw7vG3VbGz4KB2woZC2D4C2oio%3D"}
```
