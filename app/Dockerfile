FROM php:fpm
RUN pecl install xdebug \
    && docker-php-ext-enable xdebug

RUN apt-get update && apt-get install -y \
    nano
RUN mkdir /tmp/xdebug
RUN chmod 777 /tmp/xdebug