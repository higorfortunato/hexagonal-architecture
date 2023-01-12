# hexagonal-architecture

This is a demo project with the goal of demonstrate the main attributes of hexagonal architecture.

## Docker

```sh
docker-compose up -d
docker exec -it appproduct bash
docker-compose down
```

## Sqlite from Docker bash

```sh
sqlite3 db.sqlite
```

## CLI

```sh
cobra-cli init
cobra-cli add cli
go run main.go cli -a=create -n="Product CLI" -p25.0
go run main.go cli -a=get --id=e0854b6d-c349-481e-a32f-4b5e18357253
```

## WEBSERVER

```sh
cobra-cli add http
go run main.go http
```

## Testing with Postman

POST localhost:9000/product
{
"name": "Testando com Postman no",
"price": 0
}

GET localhost:9000/product/06c7378c-76ce-4b7c-b27a-ac986bc08336/enable

GET localhost:9000/product/06c7378c-76ce-4b7c-b27a-ac986bc08336/disable
