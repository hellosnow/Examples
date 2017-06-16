## Request

```http
POST https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res4167/providers/Microsoft.Storage/storageAccounts/sto3539/regenerateKey?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Length: 18
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: af91a1aa-011d-458f-ac95-86842b3cce70
host: management.azure.com
Connection: close

{"keyName":"key2"}
```

## Curl

```bash
curl -X POST 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res4167/providers/Microsoft.Storage/storageAccounts/sto3539/regenerateKey?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \ 
-H 'Content-Length: 18' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: af91a1aa-011d-458f-ac95-86842b3cce70' \
-d { \
  "keyName": "key2" \
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
x-ms-request-id: 50a088ea-19d2-41ca-aa47-a9ab497e3b9a
x-ms-correlation-request-id: 50a088ea-19d2-41ca-aa47-a9ab497e3b9a
x-ms-routing-request-id: WESTUS2:20170615T095442418Z:50a088ea-19d2-41ca-aa47-a9ab497e3b9a
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 288
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"keys":[{"keyName":"key1","permissions":"Full","value":"7xl+yQ4MrVpZCHspveCfy4f8jgTY1wv42gHO8k4bAX+EPvN4hY5uPau/bpofgeye+K9FtgvjkadkLISPfOxlMw=="},{"keyName":"key2","permissions":"Full","value":"uC+kyJ9/gT81E/+9I1Go4xtOe8sW5rdIm3n6PNIyQ5kGO5OpFq69aWnrn3jLeFIyItzpln9P392U0353RYKvbg=="}]}
```
