# DOCKER-MYSQL

Includes:
- MySQL 5.7 (port 3306)
- MySQL 8.0 (port 3307)
- PhpMyAdmin

## How to start:
Start nginx-proxy
```shell
docker network create nginx-proxy
docker run -d -p 80:80 --name proxy --network nginx-proxy -v /var/run/docker.sock:/tmp/docker.sock:ro jwilder/nginx-proxy
```
Add to `hosts` file:
```
127.0.0.1 phpmyadmin.local
127.0.0.1 phpmyadmin2.local
```
Then start MySQL
```shell

docker-compose up -d
```