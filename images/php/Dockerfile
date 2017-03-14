FROM laradock/php-fpm:7.0--1.2

MAINTAINER Mahmoud Zalt <mahmoud@zalt.me>

RUN apt-get update && apt-get install -y libmcrypt-dev
RUN pecl install mongodb-1.1.9 && \
    docker-php-ext-enable mongodb

#### SOCKET CONNECTION ####
RUN docker-php-ext-install sockets mcrypt mbstring tokenizer mysqli pdo_mysql
CMD ["php-fpm"]

EXPOSE 9000
