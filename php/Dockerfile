FROM php:8.3-apache

RUN apt-get update && apt-get install -y \
    libonig-dev vim wget \
    libfreetype6-dev \
    libjpeg62-turbo-dev \
    libwebp-dev \
    libxpm-dev \
    software-properties-common \
    && docker-php-ext-install pdo_mysql mysqli \
    && docker-php-ext-configure gd \
      --with-freetype \
      --with-jpeg \
      --with-webp \
      --with-xpm
