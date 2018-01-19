> While setting up old project i found out that laradock supporting only php>=5.6.
> But i need somehow to change php to version 5.3
> So i created a simple "rdy to go" example that can be implement in few steps 

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
