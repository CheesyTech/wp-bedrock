FROM php:7.4-fpm

RUN usermod -u 1000 www-data

RUN apt-get update \
&& docker-php-ext-install mysqli

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y git && \
    apt-get install -y unzip

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
