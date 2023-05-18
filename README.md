# Struktur Folder Project Pemrograman Web CR001 dengan tambahan database

# Cara set project

## Build menggunakan docker-compose

```shell
docker-compose up -d --build
```

## Masuk ke shell atau bash container

```shell
docker exec -it pemweb bash
```

## Install laravel 9 menggunakan shell atau bash container yg berisi php

```shell
composer create-project laravel/laravel:^9.0 .
```

## Jika error laravel log gunakan ini didalam container shell atau bash

```shell
chown -R www-data:www-data /var/www
```

## Ubah environment untuk database variable di laravel (di file .env laravel nya) 

```shell
DB_HOST=mysql_pemweb
DB_PORT=3306
DB_DATABASE=simple_crud_product
DB_USERNAME=root
DB_PASSWORD=p455w0rd
```
