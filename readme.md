## devConnect

MERN stack application to manage developers profiles

### Api

#### Register user

Endpoint: POST /api/users/login

```
curl --request POST \
  --url http://localhost:5000/api/users/login \
  --header 'accept: application/json' \
  --header 'authorization: BEARER someJWTtoken' \
  --header 'cache-control: no-cache' \
  --header 'content-type: application/json' \
  --header 'origin: http://localhost:8100' \
  --header 'postman-token: c1d4114b-8a1e-45ad-a04d-b02f55a259a3' \
  --header 'referer: http://localhost:8100/index.html' \
  --header 'user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36' \
  --data '{
	"name": "nobody",
	"email": "nobody@example.com",
	"password": "1234567"
}'
```

#### Get current user

Endpoint: GET /api/users/current

Protected route with JWT

```
curl --request GET \
  --url http://localhost:5000/api/users/current \
  --header 'accept: application/json' \
  --header 'authorization: Bearer someJWTtoken' \
  --header 'cache-control: no-cache,no-cache' \
  --header 'content-type: application/json' \
  --header 'origin: http://localhost:8100' \
  --header 'postman-token: d1c73e7a-7dd8-41bb-a4d0-1d5298004d96' \
  --data '{
	"email": "nobody@example.com",
	"password": "1234567"
}'
```
