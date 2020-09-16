FROM php:7.4.9-cli-alpine

COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer

RUN apk add --no-cache bash git

WORKDIR /app
