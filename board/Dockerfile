FROM php:5.4-apache

RUN curl -fsSL 'https://github.com/vichan-devel/vichan/archive/vichan-5.1.0.tar.gz' -o vichan.tar.gz
RUN mkdir board
RUN tar xvzf vichan.tar.gz --strip-components=1 -C board
RUN rm -rf vichan.tar.gz

RUN apt-get update
RUN apt-get install -y libonig-dev
RUN apt-get install -y libzip-dev
RUN apt-get install -y libpng-dev

RUN docker-php-ext-install gd
RUN docker-php-ext-install pdo
RUN docker-php-ext-install mbstring
