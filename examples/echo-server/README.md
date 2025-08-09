# Echo HTTP Server Example

Run a minimal HTTP server using the Echo framework.

## Run

```bash
cd examples/echo-server
go run .
```

## Test

In a separate shell:

```bash
curl -s http://localhost:1323/
# Hello, Echo!

curl -s http://localhost:1323/users/42
# {"id":"42"}

curl -s -X POST http://localhost:1323/echo -H 'Content-Type: application/json' -d '{"msg":"hi"}'
# {"msg":"hi"}
```