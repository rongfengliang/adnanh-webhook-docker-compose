# adnanh/webhook demo

## How to Run

```code
docker-compose up -d
```

## Test

```code
http://localhost:9000/hooks/simple-one?token=42
```

## shell script test

> include post args && url args

```code
curl -X POST \
  'http://localhost:9000/hooks/simple-one?token=42' \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: 1f7511f8-3a78-8092-430c-23b832df29f9' \
  -d '{
"id":"demoappaaaaddd "
}'

result:

demoappaaaaddd 42 , demoappaaaaddd , 42

```