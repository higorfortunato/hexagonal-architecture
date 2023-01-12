# hexagonal-architecture

## Docker

docker-compose up -d
docker exec -it appproduct bash
docker-compose down

### Sqlite from Docker bash

sqlite3 db.sqlite

## CLI

cobra-cli init
cobra-cli add cli
go run main.go cli -a=create -n="Product CLI" -p25.0
go run main.go cli -a=get --id=e0854b6d-c349-481e-a32f-4b5e18357253
