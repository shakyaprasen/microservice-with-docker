# Barebones microservice with docker

This repo is a sort of a template for nodejs microservices which uses Krakend as an API gateway.
Rabbitmq is also used for communication between microservices.

# Tech stack

## Nodejs
- [Nodejs](https://nodejs.org/en/docs/) is used as a backend server for both (consumer, producer) microservices.

## Krakend
- [Krakend](https://www.krakend.io/docs/overview/introduction/) is used for the API gateway, to aggregate and add rules for any API to be exposed by the nodejs microservices

## Rabbimq
- [Rabbitmq](https://www.rabbitmq.com/documentation.html) is used as a message broker between the two microservices.

## Docker
- [Docker](https://docs.docker.com/) ties up all these services and runs it using the docker-compose.yml file
