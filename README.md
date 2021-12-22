# docker4php

Docker for PHP frameworks running apache, php8, mariaDb and phpMyAdmin.

### Requirements

- Git
- Docker

### Usage

1. Clone this repo using:
```
git clone https://github.com/el-abdel/docker4php.git
```
2. Go to the repo directory:
```
cd docker4php
```
3. Start containers:
```
docker-compose up
```
> Do not forget to add virtual hosts (php-app.local, phpmyadmin.local) in your /etc/hosts file.

### Project tree

```
Work Directory
  |
  |───docker4php <===== Dockerized environnement
  │   │   .gitignore
  |   |   docker-compose.yml
  │   │   README.md
  |   |   LICENSE
  │   │
  │   └───data
  |   |     .gitignore
  |   |
  │   └───log
  |   |     .gitignore
  |   |
  │   └───etc
  |   |   │
  |   |   └───apache2
  │   |       |   
  |   |       └───sites-enabled
  │   |                php-app.local.conf
  |   |
  |   |
  |   └───images
  │       |   Dockerfile
  │       |
  |       └───config
  │              opcache.ini
  │   
  └───php-app <===== Application code source here
```
