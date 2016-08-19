FROM php:7.0-fpm

RUN apt-get update \
    && apt-get install -y git libssl-dev zlib1g-dev libicu-dev g++ \
    && pecl install apcu-5.1.5 \
    && docker-php-ext-enable apcu \
    && docker-php-ext-install zip mbstring intl opcache pdo pdo_mysql

RUN curl -sS https://getcomposer.org/installer | php \
    && mv composer.phar /usr/bin/composer
