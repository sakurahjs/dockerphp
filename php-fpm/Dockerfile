FROM php:7.2-fpm

#pdo install
RUN docker-php-ext-install pdo_mysql

#composer install
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer

#git install
RUN apt-get update
RUN apt-get install -y git

#xdebug install
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug