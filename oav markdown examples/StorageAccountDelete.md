## Request

```http
DELETE https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res4228/providers/Microsoft.Storage/storageAccounts/sto2434?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: 444d42b7-e236-4126-ab11-2b0902c1fe99
host: management.azure.com
Connection: close


```

## Curl

```bash
curl -X DELETE 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res4228/providers/Microsoft.Storage/storageAccounts/sto2434?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: 444d42b7-e236-4126-ab11-2b0902c1fe99' \
```

## Response

#### StatusCode: 200

```http
HTTP 1.1 200
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: 608c6168-2a13-4535-bafd-beddec2e5a5f
x-ms-correlation-request-id: 608c6168-2a13-4535-bafd-beddec2e5a5f
x-ms-routing-request-id: WESTUS2:20170615T095442412Z:608c6168-2a13-4535-bafd-beddec2e5a5f
Strict-Transport-Security: max-age=31536000; includeSubDomains
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

""
```
