## Request

```http
POST https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/providers/Microsoft.Storage/checkNameAvailability?api-version=2017-06-01 HTTP/1.1
Authorization: Bearer <token>
Content-Length: 61
Content-Type: application/json
accept-language: en-US
x-ms-client-request-id: 78da623d-722c-4c80-b695-0d44c2468164
host: management.azure.com
Connection: close

{"name":"sto3363","type":"Microsoft.Storage/storageAccounts"}
```

## Curl

```bash
curl -X POST 'https://management.azure.com/subscriptions/27de630f-e1ee-42de-8849-90def4986454/providers/Microsoft.Storage/checkNameAvailability?api-version=2017-06-01' \
-H 'authorization: bearer <token>' \ 
-H 'Content-Length: 61' \
-H 'Content-Type: application/json' \
-H 'accept-language: en-US' \
-H 'x-ms-client-request-id: 78da623d-722c-4c80-b695-0d44c2468164' \
-d { \
  "name": "sto3363", \
  "type": "Microsoft.Storage/storageAccounts" \
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
x-ms-request-id: b064cf04-9928-4b91-96df-8889170755b0
x-ms-correlation-request-id: b064cf04-9928-4b91-96df-8889170755b0
x-ms-routing-request-id: WESTUS2:20170615T095442409Z:b064cf04-9928-4b91-96df-8889170755b0
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Length: 22
content-type: application/json
Date: Thu, 15 Jun 2017 09:54:42 GMT
Connection: close

{"nameAvailable":true}
```
