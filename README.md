# Sock Shop : A Microservice Demo Application


This is a forked repository of: 
[Link to Repo](https://github.com/microservices-demo/microservices-demo)

We modified the original project as part of our MasterFachstudie.
All modifications are included in this repository.

## Installation
In order to run the application, you have to build several services locally.
(they are not hosted as images on the demo repository)

The following services have to be build locally:

- orders
- ordersProcess
- Sockenshop_API_Gateway
- front-end


## Start
```
docker-compose -f deploy/docker-compose/docker-compose.yml up -d
```

## Shutdown 
```
docker-compose -f deploy/docker-compose/docker-compose.yml down
```

## Tests 
```
docker run --net=host weaveworksdemos/load-test -h localhost -r 100 -c 2
```
