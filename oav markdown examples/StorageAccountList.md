## Request

```http
GET https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/providers/Microsoft.Storage/storageAccounts?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: d6609a31-edcb-4623-9cb2-b165f1e341f4
host: management.azure.com
Connection: close


```

## Curl

```bash
curl -X GET 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/providers/Microsoft.Storage/storageAccounts?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: d6609a31-edcb-4623-9cb2-b165f1e341f4' \
```

## Response

#### StatusCode: 200

```http
HTTP 1.1 200
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: fc7e882a-07eb-472f-9f0f-9e6e39c93d77
x-ms-correlation-request-id: fc7e882a-07eb-472f-9f0f-9e6e39c93d77
x-ms-routing-request-id: WESTUS2:20170615T095442414Z:fc7e882a-07eb-472f-9f0f-9e6e39c93d77
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 4428
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"value":[{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res2627/providers/Microsoft.Storage/storageAccounts/sto1125","kind":"Storage","location":"eastus2euap","name":"sto1125","properties":{"creationTime":"2017-05-24T13:28:53.4540398Z","primaryEndpoints":{"blob":"https://sto1125.blob.core.windows.net/","file":"https://sto1125.file.core.windows.net/","queue":"https://sto1125.queue.core.windows.net/","table":"https://sto1125.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"},{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/testcmk3/providers/Microsoft.Storage/storageAccounts/sto3699","identity":{"principalId":"356d057d-cba5-44dd-8a30-b2e547bc416b","tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47","type":"SystemAssigned"},"kind":"Storage","location":"eastus2euap","name":"sto3699","properties":{"creationTime":"2017-05-24T10:06:30.6093014Z","primaryEndpoints":{"blob":"https://sto3699.blob.core.windows.net/","file":"https://sto3699.file.core.windows.net/","queue":"https://sto3699.queue.core.windows.net/","table":"https://sto3699.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"},{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/testcmk3/providers/Microsoft.Storage/storageAccounts/sto6637","identity":{"principalId":"911871cc-ffd1-4fc4-ac11-7a316433ea66","tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47","type":"SystemAssigned"},"kind":"Storage","location":"eastus2euap","name":"sto6637","properties":{"creationTime":"2017-05-24T10:09:39.5625175Z","primaryEndpoints":{"blob":"https://sto6637.blob.core.windows.net/","file":"https://sto6637.file.core.windows.net/","queue":"https://sto6637.queue.core.windows.net/","table":"https://sto6637.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"},{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res8186/providers/Microsoft.Storage/storageAccounts/sto834","kind":"Storage","location":"eastus2euap","name":"sto834","properties":{"creationTime":"2017-05-24T13:28:20.8686541Z","primaryEndpoints":{"blob":"https://sto834.blob.core.windows.net/","file":"https://sto834.file.core.windows.net/","queue":"https://sto834.queue.core.windows.net/","table":"https://sto834.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"},{"id":"/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/testcmk3/providers/Microsoft.Storage/storageAccounts/sto9174","identity":{"principalId":"933e3ddf-1802-4a51-9469-18a33b576f88","tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47","type":"SystemAssigned"},"kind":"Storage","location":"eastus2euap","name":"sto9174","properties":{"creationTime":"2017-05-24T09:46:19.6556989Z","primaryEndpoints":{"blob":"https://sto9174.blob.core.windows.net/","file":"https://sto9174.file.core.windows.net/","queue":"https://sto9174.queue.core.windows.net/","table":"https://sto9174.table.core.windows.net/"},"primaryLocation":"eastus2euap","provisioningState":"Succeeded","secondaryLocation":"centraluseuap","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"}]}
```
