FROM php:7.4.9-fpm-alpine as fpm

RUN apk --no-cache add postgresql-dev pcre-dev ${PHPIZE_DEPS}

RUN docker-php-ext-install pdo_pgsql

RUN pecl install xdebug

FROM fpm AS xdebug

RUN docker-php-ext-enable xdebug

COPY xdebug/php.ini "/usr/local/etc/php/conf.d/"