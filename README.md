# Nina

- <https://www.youtube.com/watch?v=SXwC9fSwct8>

## Docker run (mongodb)

``` bash
docker run -d -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=root --network mongo-network --name mongodb mongo
```

## Docker run (mongo-express)

``` bash
docker run -d -p 8081:8081 -e ME_CONFIG_MONGODB_ADMINUSERNAME=admin -e ME_CONFIG_MONGODB_ADMINPASSWORD=root -e ME_CONFIG_MONGODB_SERVER=mongodb --network mongo-network --name mongo-express mongo-express
```
