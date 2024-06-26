# an image to compile and run java code in a container using openjdk-17-jdk
FROM php:8.0-fpm-alpine

RUN apk update && \
    apk add --no-cache git curl bash && \
    docker-php-ext-install pdo_mysql

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

COPY ./laravel-boilerplate/ /var/www/laravel-boilerplate

# RUN git clone https://github.com/rappasoft/laravel-boilerplate.git /var/www/laravel-boilerplate

WORKDIR /var/www/laravel-boilerplate

# RUN composer install

# RUN cp .env.example .env && php artisan key:generate

# EXPOSE 80

# CMD php artisan serve --host=0.0.0.0 --port=80

# Entry point for the container, launch shell
CMD ["/bin/sh"]