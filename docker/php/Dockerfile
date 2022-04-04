FROM php:8.0-fpm

RUN apt update
RUN apt install -y wget git unzip libpq-dev
RUN apt install -y zlib1g-dev mariadb-client libzip-dev libonig-dev \
  && docker-php-ext-install zip pdo_mysql


# Install Node.js 12
RUN apt install -y npm \
  && npm install n -g \
  && n 12

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php \
  && mv composer.phar /usr/local/bin/composer \
  && composer self-update 2.3.3

WORKDIR /var/www