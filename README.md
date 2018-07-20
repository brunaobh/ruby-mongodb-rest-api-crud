# A simple *Ruby app - REST API* connected to a NOSQL MongoDB Database

Note:__ This isn't production-ready code. The service assumes no Mongo username/password, doesn't force SSL, or enforce security best practices. This is for demonstration and learning purposes only. 

## Introduction

Feel free to use, comment and contribute


## Instructions

# Running locally using Docker

Use docker-compose to build the service and mongodb containers (takes a few minutes the first time):

> docker-compose build

Then start the the containers:

> docker-compose up

## How to use

Get a list of products (empty by default):

> curl -X GET http://127.0.0.1:4567/products

Add a new product:

> curl -X POST http://127.0.0.1:4567/products -F "name=My Product"