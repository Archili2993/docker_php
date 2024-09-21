FROM php:8.1-fpm-alpine

RUN apk add --no-cache \
    $PHPIZE_DEPS \
    mysql-dev \
    && docker-php-ext-install pdo pdo_mysql \
    && docker-php-ext-enable pdo pdo_mysql \
    && apk del $PHPIZE_DEPS