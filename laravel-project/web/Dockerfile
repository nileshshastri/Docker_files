FROM php:7.2-fpm
RUN apt-get update && apt-get install -y \
    build-essential \
    default-mysql-client \
    libpng-dev \
    libjpeg62-turbo-dev \
    libfreetype6-dev \
    locales \
    zip \
    jpegoptim optipng pngquant gifsicle \
    vim \
    unzip \
    git \
    curl

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composerRUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

COPY . /var/www
#RUN cd /var/www/laravel-app/v1/ \
#    && composer require guzzlehttp/guzzle \
#    && composer require aws/aws-sdk-php \
#    && php artisan optimize:clear \ 
#    && cd /var/www/laravel-root/v1/ \
#    && composer require guzzlehttp/guzzle \
#    && composer require aws/aws-sdk-php \
#    && php artisan optimize:clear 
