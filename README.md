# BITS-estore
BITS Scalable Services Assignment 1

This app is composed of 3 microservices: 
1. Estore (Frontend gateway in angular and backend module to connect to other microservices, BFF Pattern in short)
2. Invoice Microservice (Backend microservice in java) 
3. Notification Microservice (Backend microservice in java and mongodb)

In order to run this app, the following are the prerequisites: 
* First run the Jhipster registry service by running the follwing command in folder estore:
`docker-compose -f src/main/docker/jhipster-registry.yml up -d`
* For running notification service seamlessly you'll need a mongo db up and running, hence run the below command in the folder `notification`:
`docker-compose -f src/main/docker/mongodb.yml up -d`
* Then run the Jhipster control center for monitoring the services (OPTIONAL)
`docker-compose -f src/main/docker/jhipster-control-center.yml up -d`

After running the above commands, move to each microservice directory and run `./gradlew` in mac or linux or `gradlew` in windows and your application would be up and running. 
