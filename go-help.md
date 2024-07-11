# go commands

```bash
# iniciar um projeto go
go mod init journey
```

```bash
# instalar os pacotes que faltam
go mod tidy

# baixar a ultima versão dos pacotes
go get -u ./ ...

# rodar o arquivo gen
go generate ./ ....
```

## gerar interfaces
VsCode -> ctrl + shift + P -> Go: Generate Interface Stubs
colocar o "Receiver" + o package e o nome da interface que quer implementar
ex: api API spec.ServerInterface 

# database commands

## migrations

```bash
# using github.com/jackc/tern package
tern init ./internal/pgstore/migrations

# criar uma migration
tern new --migrations ./internal/pgstore/migrations create_trips_table

# executar as migrations
tern migrate --migrations ./internal/pgstore/migrations --config ./internal/pgstore/migrations/tern.conf
```

## sqlc

```bash
# criar as queries através do sql
sqlc generate -f ./internal/pgstore/sqlc.yaml
```
  