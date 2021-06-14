# DOCKER-MYSQL

Includes:
- MySQL 5.7 (port 3306)
- MySQL 8.0 (port 3307)
- PhpMyAdmin (http://127.0.0.1:8081/)

How to start:
```shell
docker-compose up -d
```

Connect to multiple servers at once (in separate tabs):
```shell
docker-compose up -d --scale phpmyadmin=2
```

PhpMyAdmin instances:  
http://127.0.0.1:8081/  
http://127.0.0.1:8082/