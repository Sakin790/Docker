# To run this script
```
docker-compose up -d
```

##### Access the PostgreSQL Container Use the container name postgres_container to open a terminal session inside it:

```
docker exec -it postgres_container bash
```
## Connect to PostgreSQL Database

```
psql -U root -d test_db
```