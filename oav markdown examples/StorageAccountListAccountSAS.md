## Request

```http
POST https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res7985/providers/Microsoft.Storage/storageAccounts/sto8588/ListAccountSas?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Length: 211
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: d628ead6-22aa-4226-b5b4-17482efd2714
host: management.azure.com
Connection: close

{"signedServices":"b","signedResourceTypes":"s","signedPermission":"r","signedProtocol":"https,http","signedStart":"2017-05-24T10:42:03.1567373Z","signedExpiry":"2017-05-24T11:42:03.1567373Z","keyToSign":"key1"}
```

## Curl

```bash
curl -X POST 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res7985/providers/Microsoft.Storage/storageAccounts/sto8588/ListAccountSas?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \ 
-H 'Content-Length: 211' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: d628ead6-22aa-4226-b5b4-17482efd2714' \
-d { \
  "signedServices": "b", \
  "signedResourceTypes": "s", \
  "signedPermission": "r", \
  "signedProtocol": "https,http", \
  "signedStart": "2017-05-24T10:42:03.1567373Z", \
  "signedExpiry": "2017-05-24T11:42:03.1567373Z", \
  "keyToSign": "key1" \
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
x-ms-request-id: 10e35cde-1028-461a-95f5-b1d2464958f9
x-ms-correlation-request-id: 10e35cde-1028-461a-95f5-b1d2464958f9
x-ms-routing-request-id: WESTUS2:20170615T095442420Z:10e35cde-1028-461a-95f5-b1d2464958f9
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 179
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"accountSasToken":"sv=2015-04-05&ss=b&srt=s&sp=r&st=2017-05-24T10%3A42%3A03Z&se=2017-05-24T11%3A42%3A03Z&spr=https,http&sig=Z0I%2BEpM%2BPPlTC8ApfUf%2BcffO2aahMgZim3U0iArqsS0%3D"}
```
