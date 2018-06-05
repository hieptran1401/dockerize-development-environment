FROM php:7.2.6-fpm-alpine3.7

RUN apk update && apk add \
        curl-dev \
        libzip-dev \
        freetype-dev \
        libjpeg-turbo-dev \
        libpng-dev \
        libxml2-dev \
        gettext-dev \
    && docker-php-ext-install -j$(nproc) mysqli pdo pdo_mysql zip gd mbstring xml curl json gettext tokenizer