docker exec -it <container_name_or_id> /bin/bash

# Install nignx
```
apt install nginx
apt install nginx
ufw app list
```
# Kafka
```
version: '3'
services:
  image:confluentinc/cp-kafka
  port: '-9092:9092'
  enviroment:
   KAFKA_ENVIROMENT_CONNECT:""
```