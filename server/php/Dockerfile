FROM php:7.3-fpm

# Install dependencies
RUN apt-get update && apt-get install -y \
    sudo \
    libxml2-dev \
    libicu-dev \
    libjpeg62-turbo-dev \
    libmcrypt-dev \
    libpng-dev \
    libxslt1-dev \
    sendmail-bin \
    sendmail \
    libzip-dev \
    libonig-dev \
\
# Install required php extensions
 && docker-php-ext-install \
    pdo \
    pdo_mysql \
    dom \ 
    gd \ 
    intl \ 
    mbstring \ 
    pdo_mysql \ 
    xsl \ 
    zip \ 
    soap \ 
    bcmath \ 
    pcntl \ 
    sockets \
\
# Install composer
 && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer --version=1.10.10
