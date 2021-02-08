### MongoDB

#### Download Docker for MongoDB

`docker pull mongo`

#### Run Docker for MongoDB (using port 27017, name mongo)

`docker run -d -p 27017:27017 --name mongo mongo`

#### Run MongoShell on Docker Instance

`docker exec -it mongo bash`
`mongo`

#### Execute MongoShell Commands

`show dbs`
`use local`
`db.startup_log.count();`

### Accessing Data with MongoDB and Spring

#### Tutorial for Spring and MongoDB

https://spring.io/guides/gs/accessing-data-mongodb/

#### Download Example

Export src/main/java/hello/* to src/main/java/customer/* and pom.xml

#### Build and Run Exmample

`mvn clean install`
`mvn spring-boot:run `
`     -Dspring.data.mongodb.uri=mongodb://localhost:27017/customer`

#### Check Data in MongoDB

`docker exec -it mongo bash`
`mongo`
`use customer`
`db.customer.find()`

