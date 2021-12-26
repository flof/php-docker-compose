FROM php:8.0-fpm
RUN php -r "readfile('http://getcomposer.org/installer');" | php -- --install-dir=/usr/bin/ --filename=composer
RUN apt update && apt install -y zip unzip wget zlib1g-dev libicu-dev libpng-dev cron
RUN docker-php-ext-install mysqli pdo_mysql intl opcache gd
RUN mv "$PHP_INI_DIR/php.ini-production" "$PHP_INI_DIR/php.ini"
