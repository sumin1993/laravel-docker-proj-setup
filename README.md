# Laravel + Nginx + Docker

## Description
Start developing a fresh Laravel application with `docker` using `docker-compose`.

The images used in this repo is `nginx`,`mysql:5.7` and `laravel 6.*`. 
The goal is to make setting up the development as simple as possible.

laravel version 6.* install command
```
composer create-project --prefer-dist laravel/laravel blog "6.*"
```

## 1. Setup development environment
### Prerequisites
In order to use this compose file (docker-compose.yml) you must have:

1. [docker](https://docs.docker.com/engine/installation/)
1. [docker-compose](https://docs.docker.com/compose/install/)

## 2. Build the images and start the services:
* all the docker setup environment done and just run the services.
```
docker-compose build
docker-compose up -d
```

## 3. Run Project 
```
docker exec app php artisan migrate

・phpmyadmin
http://localhost:8100/
db: laravel
username: user1
password: admin

・laravel project
http://localhost:8000/
```