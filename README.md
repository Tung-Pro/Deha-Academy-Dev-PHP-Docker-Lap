Nguyễn Văn Tùng

Deha-Academy-Docker-Lap1

## Getting Started
`git clone https://github.com/Tung-Pro/Deha-Academy-Docker-Lap1 ` </br>

` cd Deha-Academy-Docker-Lap1 ` </br>

` git clone https://github.com/Laradock/laradock.git ` </br>

`cd laradock`

## Tạo .env 

`cp .env.example .env`</br>

Edit .env: </br>

APP_CODE_PATH_HOST=../app

NGINX_HOST_HTTP_PORT=8989

## Sửa NGINX 

`cd nginx/sites` </br>

Edit default.conf: </b>

root /var/www/laravel/public;

## Tạo Lavavel và index.php

`cd laradock`

`docker-compose up -d nginx workspace`

`docker-compose exec workspace bash`

`composer create-project laravel/laravel laravel`

`touch index.php`

index.php:

Hello Docker!

`exit`

## Sử dụng Docker image: nginx, php, mysql, sử dụng Dockerfile và Docker compose tạo môi trường chạy ứng dụng PHP.
`docker-compose down`

`cd ~/Deha-Academy-Docker-Lap1`

`docker-compose up -d`

http://localhost:5000

![image](https://github.com/user-attachments/assets/21d878ec-0201-4beb-bff4-3a486dce034c)

## Sử dụng Laradock tạo môi trường chạy Laravel, thay đổi được cấu hình (port, version PHP) Laradock.

`docker-compose down`

`cd laradock`

`docker-compose up -d nginx`

http://localhost:8686

![image](https://github.com/user-attachments/assets/e995ba84-da56-4a3d-adfa-523605e5674e)



