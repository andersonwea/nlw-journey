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
```

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
  