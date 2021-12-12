# Docker - Laravel - Apache - MySql

-   Laravel 8
-   PHP 8
-   MySql 5.7

## Description

Start developing a fresh Laravel application with `docker` using `docker-compose`.

The images used in this repo is `php:8.0-apache` and `mysql:5.7`. The goal is to make setting up the development as simple as possible.

Laravel setup with Docker

#### Installation

```
git clone git@github.com:bhavin-nakrani/Docker-Laravel-Apache-MySql.git laravel-app

cd laravel-app

cp .env.example .env
```

Build the images and start the services:

```
docker-compose build
docker-compose up -d
```

#### Connect with container

```
docker exec -it laravel-app bash -c "sudo -u devuser /bin/bash"

composer install

php artisan key:generate

```

#### Connect with database

```
docker exec -it mysql-db bash -c "mysql -u laravel -p laravel"

```

Server URL:

http://localhost:8080/
