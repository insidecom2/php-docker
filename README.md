# How to use

1. make folder mysql_data
   `$sh touch mysql_data`
2. make folder schema
   `$sh touch schema`
3. run docker-compose up
   `$sh docker-compose up` for run normal
   ` $sh docker-compose up -d` for run ob backgroup (demon)

# Config

Change version of php , go to Dockerfile , change version of php
`FROM php:7.4-apache` change version you want.

Change folder work
Dockerfile
`COPY ./wordpress /var/www/html/` change wordpress to another folder or . (for root path)
docker-compose.yml
`volumes: `
`      - ./wordpress:/var/www/html` change wordpress to another folder or . (for root path)
