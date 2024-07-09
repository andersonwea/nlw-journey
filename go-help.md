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
```
  