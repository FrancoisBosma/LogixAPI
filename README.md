# LogixAPI

## Get Schema from curl
```bash
curl "http://localhost:8080/admin" -H "Content-Type: application/json" --data-binary '{"query":"{\n getGQLSchema {\n schema\n generatedSchema\n }\n}","variables":{}}' --compressed
```
## Otherwise use a client like [Altair](https://github.com/altair-graphql/altair)

## Update Schema w/ curl
```bash
curl -X POST localhost:8080/admin/schema --data-binary '@schema.gql' --compressed
```
