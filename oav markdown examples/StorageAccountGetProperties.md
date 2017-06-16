## Request

```http
GET https://management.azure.com/subscriptions/45b60d85-fd72-427a-a708-f994d26e593e/resourceGroups/res9407/providers/Microsoft.Storage/storageAccounts/sto8596?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: 57387da5-7be6-4d25-847c-85ae98256a87
host: management.azure.com
Connection: close


```

## Curl

```bash
curl -X GET 'https://management.azure.com/subscriptions/45b60d85-fd72-427a-a708-f994d26e593e/resourceGroups/res9407/providers/Microsoft.Storage/storageAccounts/sto8596?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: 57387da5-7be6-4d25-847c-85ae98256a87' \
```

## Response

#### StatusCode: 200

```http
HTTP 1.1 200
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: 9e75b7eb-4381-4ce5-806b-6acbd908ebb8
x-ms-correlation-request-id: 9e75b7eb-4381-4ce5-806b-6acbd908ebb8
x-ms-routing-request-id: WESTUS2:20170615T095442413Z:9e75b7eb-4381-4ce5-806b-6acbd908ebb8
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 916
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"id":"/subscriptions/45b60d85-fd72-427a-a708-f994d26e593e/resourceGroups/res9407/providers/Microsoft.Storage/storageAccounts/sto8596","kind":"Storage","location":"eastus2(stage)","name":"sto8596","properties":{"creationTime":"2017-06-01T02:42:41.7633306Z","networkAcls":{"bypass":"AzureServices","defaultAction":"Allow","ipRules":[],"virtualNetworkRules":[]},"primaryEndpoints":{"blob":"https://sto8596.blob.core.windows.net/","file":"https://sto8596.file.core.windows.net/","queue":"https://sto8596.queue.core.windows.net/","table":"https://sto8596.table.core.windows.net/"},"primaryLocation":"eastus2(stage)","provisioningState":"Succeeded","secondaryLocation":"northcentralus(stage)","statusOfPrimary":"available","statusOfSecondary":"available","supportsHttpsTrafficOnly":false},"sku":{"name":"Standard_GRS","tier":"Standard"},"tags":{"key1":"value1","key2":"value2"},"type":"Microsoft.Storage/storageAccounts"}
```
