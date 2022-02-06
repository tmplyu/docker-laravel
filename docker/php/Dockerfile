FROM php:8.0-fpm

ENV TZ Asia/Tokyo

RUN apt update && apt install -y \
       libzip-dev \
    && docker-php-ext-install zip pdo_mysql

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

RUN pecl install xdebug \
    && docker-php-ext-enable xdebug
