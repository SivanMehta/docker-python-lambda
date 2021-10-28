## run locally

```sh
# build container locally
docker build -t dummy .
docker run -p 9000:8080 dummy
```

You can now access the application at http://localhost:9000/ or via `curl`:

```sh
curl -XPOST "http://localhost:9000/2015-03-31/functions/function/invocations" -d '{"payload":"hello world!"}'
```
