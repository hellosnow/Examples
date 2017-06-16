## Request

```http
POST https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res418/providers/Microsoft.Storage/storageAccounts/sto2220/listKeys?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: 3e13423f-25cd-4f0a-aabe-6096152aa04c
host: management.azure.com
Connection: close


```

## Curl

```bash
curl -X POST 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/resourceGroups/res418/providers/Microsoft.Storage/storageAccounts/sto2220/listKeys?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: 3e13423f-25cd-4f0a-aabe-6096152aa04c' \
```

## Response

#### StatusCode: 200

```http
HTTP 1.1 200
Cache-Control: no-cache
Pragma: no-cache
Expires: -1
x-ms-ratelimit-remaining-subscription-writes: 1199
x-ms-request-id: ca851b24-342b-4b7c-a509-cadbb4698d25
x-ms-correlation-request-id: ca851b24-342b-4b7c-a509-cadbb4698d25
x-ms-routing-request-id: WESTUS2:20170615T095442417Z:ca851b24-342b-4b7c-a509-cadbb4698d25
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 288
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"keys":[{"keyName":"key1","permissions":"Full","value":"nVF7aKIvr9mV/RM5lOD0sYoi8ThXTRHQP7o66hvUmjCDkPKR3qxPu/otJcNciz2aQdqPuzJH3ECG4TU2yZjQ7Q=="},{"keyName":"key2","permissions":"Full","value":"dNJvKnULO586Ji3nFzB7987TJs4ovnGZhyGXeiVQ75HZGPhBmBfe8lXrI7EfyATff6S5ucxffCoEAQOWbmPK/Q=="}]}
```
