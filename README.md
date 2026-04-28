# demo_webapp_nodejs_mongo_db
This repo contains files related to demo_webapp_nodejs_mongo_db


# Commands to deploy this app:
1. docker network create my-net
2. docker container run -d -p 27017:27017 --name=mongo --network=my-net mongo
3. docker conatainer run -d -p 9081:3000 --name=webapp-mongodb --network=my-net liteshz/webapp-demo-nodejs-mongodb
4. List out containers & images
 a. docker images
 b. docker container ls -a


# Notes: 
1. Use latest tag when playing with docker images & containers
2. Use v1 tag when running webapp & mongo in same container using kubernetes deployment & svc. 


# Refer below docker registry
https://hub.docker.com/repository/docker/liteshz/webapp-demo-nodejs-mongodb/tags
