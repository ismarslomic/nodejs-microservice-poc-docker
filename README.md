# nodejs-microservice-poc-docker
Files for creating docker containers for running the nodejs-microservice-poc 

## Get started
```YAML
# 1. make sure you are at top level of this folder
# 2. build all images (Docker-Compose does not automatically update images if Dockerfiles has changed)
build images: docker-compose build
# 3. create and start the containers
docker-compose up -d
```

## microservice folder
* Contains the Dockerfile for the nodejs-microservice-poc project

## mongo folder
* Contains the folder for database files that will be mounted as volume when starting mongo Docker container
* No Dockerfile defined for mongoDB since official Docker image for mongoDB is sufficient for our case

## mongo-express folder
* Contains the Dockerfile for mongo-express project

## docker-compose.yml
* Docker-Compose file that defines and runs all Dockerfiles. Read more at https://docs.docker.com/compose/yml/ and 
https://docs.docker.com/compose/