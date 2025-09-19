FROM php:8.4-apache

RUN docker-php-ext-install -j $(nproc) pdo_mysql

RUN useradd -ms /bin/bash admin
COPY --chown=admin:admin www/uploads /var/www/html/uploads

COPY www /var/www/html