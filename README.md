# Setup

  - Clone original repo from laradock by typing:
```sh
    git clone https://github.com/Laradock/laradock.git
```
  - create .env file
```sh
    cp env-example .env
```
  - replace php-fpm and workbanch folders from original laradock folder to the same folder from this repo
  - change PHP_VERSION in .env to PHP_VERSION=53
  - up containers:
```sh
    docker-compose up -d php-fpm
```
  - you can make sure, that u have right version of php by typing:
```sh
    docker-compose exec php-fpm bash
    php -v
```
