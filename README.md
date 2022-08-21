# LogixAPI

## Get Schema
```bash
curl "http://localhost:8080/admin" -H "Content-Type: application/json" --data-binary '{"query":"{\n getGQLSchema {\n schema\n generatedSchema\n }\n}","variables":{}}' --compressed
```

## Update Schema
```bash
curl -X POST localhost:8080/admin/schema --data-binary '@schema.gql' --compressed
```
