# DOCKER-MYSQL

Includes:
- MySQL 5.7 (port 3306)
- MySQL 8.0 (port 3307)
- PhpMyAdmin (ports 8081 and 8082)

## How to start:
1. Start containers: `docker-compose up -d`
2. Then open phpmyadmin: http://127.0.0.1:8081
3. Server: `mysql-5.7` or `mysql-8.0`
4. Login: `root` (without password)

## PhpMyAdmin notes
1. PhpMyAdmin instance works in [arbitrary mode](https://docs.phpmyadmin.net/en/latest/config.html#cfg_AllowArbitraryServer), so you can use it to connect to any other mysql server.
2. Second instance of PhpMyAdmin (http://127.0.0.1:8082) can be useful when you want to work with multiple servers at the same time.