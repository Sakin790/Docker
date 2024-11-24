# MongoDB
 ### Pull images Not Port Mapping
```
docker run -d --rm --name mongo-container -e MONGO_INITDB_ROOT_USERNAME='root' -e MONGO_INITDB_ROOT_PASSWORD='secret' mongo
```
# Port Mapping
```
docker run -d --rm --name mongo-container -e MONGO_INITDB_ROOT_USERNAME='root' -e MONGO_INITDB_ROOT_PASSWORD='secret' -p 27017:27017 mongo
```
# volume Bind
```
docker run -d --rm --name mongo-container -e MONGO_INITDB_ROOT_USERNAME='root' -e MONGO_INITDB_ROOT_PASSWORD='secret' -p 27017:27017 -v mongoData:/data/db mongo

```
### Run 
```
docker exec -it mongo-container bash
```
### Mongosh
```
mongosh -u root -p secret
```
# Extra
```
Here is All user Info
use admin
db.getUsers()
```
# Stop
```
docker stop mongo-container
```