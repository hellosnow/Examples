## Request

```http
PUT https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res9101/providers/Microsoft.Storage/storageAccounts/sto4445?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Length: 114
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: 0fe27581-db43-4f0f-a4b7-aee5065742b5
host: management.azure.com
Connection: close

{"sku":{"name":"Standard_GRS"},"kind":"Storage","location":"eastus2euap","tags":{"key1":"value1","key2":"value2"}}
```

## Curl

```bash
curl -X PUT 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res9101/providers/Microsoft.Storage/storageAccounts/sto4445?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \ 
-H 'Content-Length: 114' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: 0fe27581-db43-4f0f-a4b7-aee5065742b5' \
-d { \
  "sku": { \
    "name": "Standard_GRS" \
  }, \
  "kind": "Storage", \
  "location": "eastus2euap", \
  "tags": { \
    "key1": "value1", \
    "key2": "value2" \
  } \
}
```

## Initial Response

#### StatusCode: 202

```http
HTTP 1.1 202
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: d9bf30a7-a17f-49e0-bed2-4ef4495de43f
x-ms-correlation-request-id: d9bf30a7-a17f-49e0-bed2-4ef4495de43f
x-ms-routing-request-id: WESTUS2:20170615T095442411Z:d9bf30a7-a17f-49e0-bed2-4ef4495de43f
Strict-Transport-Security: max-age=31536000; includeSubDomains
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

""
```

## Final Response after polling is complete and successful

#### StatusCode: 200

```http
HTTP 1.1 200
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: b6be7462-7a3e-463b-a194-ff7c2e36ad28
x-ms-correlation-request-id: b6be7462-7a3e-463b-a194-ff7c2e36ad28
x-ms-routing-request-id: WESTUS2:20170615T095442411Z:b6be7462-7a3e-463b-a194-ff7c2e36ad28
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 799
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res9101/providers/Microsoft.Storage/storageAccounts/sto4445","kind":"Storage","location":"eastus2euap","name":"sto4445","properties":{"creationTime":"2017-05-24T13:25:33.4863236Z","primaryEndpoints":{"blob":"https://sto4445.blob.core.windows.net/","file":"https://sto4445.file.core.windows.net/","queue":"https://sto4445.queue.core.windows.net/","table":"https://sto4445.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"}
```
