## First
connect to postgres:
``` bash
psql -U postgres
```

if table not exists:
``` bash
create table person(name varchar(40), nickname varchar(40))
```

## Run server
``` bash
go mod init example.com/m/v2
go mod vendor
go run maain.go
```

## API routes

List all person record 
- GET: http://localhost:8010

Persist a person
- POST: http://localhost:8010/insert
``` bash
{
  "name": "string",
   "nickname": "string"
}
```
