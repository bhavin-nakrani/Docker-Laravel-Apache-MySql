# Docker-Laravel-Apache-MySql

Laravel setup with Docker

### Installation

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
