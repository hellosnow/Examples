## Request

```http
GET https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res6117/providers/Microsoft.Storage/storageAccounts?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: b0492d2e-0517-4aa0-b8b3-0a051b83bda2
host: management.azure.com
Connection: close


```

## Curl

```bash
curl -X GET 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res6117/providers/Microsoft.Storage/storageAccounts?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: b0492d2e-0517-4aa0-b8b3-0a051b83bda2' \
```

## Response

#### StatusCode: 200

```http
HTTP 1.1 200
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: b619b9b2-b8b2-457e-9640-f58f5f6acf37
x-ms-correlation-request-id: b619b9b2-b8b2-457e-9640-f58f5f6acf37
x-ms-routing-request-id: WESTUS2:20170615T095442415Z:b619b9b2-b8b2-457e-9640-f58f5f6acf37
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 1610
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"value":[{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res6117/providers/Microsoft.Storage/storageAccounts/sto4036","kind":"Storage","location":"eastus2euap","name":"sto4036","properties":{"creationTime":"2017-05-24T13:24:47.818801Z","primaryEndpoints":{"blob":"https://sto4036.blob.core.windows.net/","file":"https://sto4036.file.core.windows.net/","queue":"https://sto4036.queue.core.windows.net/","table":"https://sto4036.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"},{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res6117/providers/Microsoft.Storage/storageAccounts/sto4452","kind":"Storage","location":"eastus2euap","name":"sto4452","properties":{"creationTime":"2017-05-24T13:24:15.7068366Z","primaryEndpoints":{"blob":"https://sto4452.blob.core.windows.net/","file":"https://sto4452.file.core.windows.net/","queue":"https://sto4452.queue.core.windows.net/","table":"https://sto4452.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"}]}
```
