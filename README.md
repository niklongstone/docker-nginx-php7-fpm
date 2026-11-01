docker-php7-fpm-nginx
=====================

> **Discontinued:** this repository is no longer maintained. Despite the name, it now runs PHP 8.4, because PHP 7 is end-of-life and has no official fix for CVE-2026-109618 and CVE-2026-109619.

A simple Docker stack that includes:
 - Nginx
 - Mysql
 - PHP 8.4 FPM 

The configuration works for a symfony project but can be changed easily (just edit `nginx/app.conf`).  

# Installation

 - Clone this repository.
 - Insert your Symfony project under app.
 - Run `docker compose up --build`.
