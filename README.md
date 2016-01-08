docker-php7-fpm-nginx
=====================

A simple Docker stack that includes:
 - Nginx
 - Mysql
 - PHP 7 FPM 

The configuration works for a symfony project but can be changed easily (just edit `nginx/app.conf`).  

# Installation

 - Clone this repository.
 - Insert your Symfony project under app.
 - Run `docker-compose up`.
