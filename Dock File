# Dockerfile for PHP Backend
FROM php:8.0-fpm
WORKDIR /var/www
COPY ./backend /var/www
RUN docker-php-ext-install pdo pdo_mysql
