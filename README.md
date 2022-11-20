# docker_LEMP
This project was created as part of the DevOps_15802 training course

## Aim of the project
You need to run the site from this [repository](https://github.com/mentorchita/Blood-Bank-Management-System) using Docker Compose

## Installation
1. Clone this repository to localhost:
```sh
git clone https://github.com/abozhchenko/docker_LEMP.git
```
2. Edit credentials in files `.env` and `./app/files/connection.php` 
```sh
cd ./docker_LEMP
vi .env
vi ./app/files/connection.php
```
3. Start the project
```sh
docker compose up -d
```
4. Open phpMyAdmin and import `./SQL/BloodBank.sql` into `bloodbank` database
```sh
http://<ip-dockerhost>:8080
```
5. Go to webpage 
```sh
http://<ip-dockerhost>
```

## Sources
- [NGINX](https://hub.docker.com/_/nginx)
- [PHP-FPM](https://hub.docker.com/r/bitnami/php-fpm)
- [MariaDB](https://hub.docker.com/_/mariadb)
- [phpMyAdmin](https://hub.docker.com/_/phpmyadmin)
