FROM php:8.4.27-fpm-trixie

MAINTAINER Nicola Pietroluongo <nik.longstone@gmail.com>

RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libpng-dev \
    	&& docker-php-ext-configure gd --with-freetype --with-jpeg \
    	&& docker-php-ext-install gd \
        && docker-php-ext-install pdo_mysql

COPY symfony.pool.conf  /usr/local/etc/
COPY security.ini /usr/local/etc/php/conf.d/

RUN usermod -u 1000 www-data

EXPOSE 9000
CMD ["php-fpm", "-F"]
