FROM php:8.2-apache
RUN apt-get update && apt-get install -y \
    libicu-dev \
    libpq-dev \
    libzip-dev \
    zip \
    && docker-php-ext-install \
    intl \
    opcache \
    pdo \
    pdo_pgsql \
    pgsql \
    zip \
    pdo_mysql \
    mysqli \
    && a2enmod rewrite \
    && rm -rf /var/lib/apt/lists/*