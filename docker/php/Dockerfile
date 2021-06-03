FROM php:8-fpm
# install composer
RUN cd /usr/bin && curl -s http://getcomposer.org/installer | php && ln -s /usr/bin/composer.phar /usr/bin/composer
RUN apt-get update \
    && apt-get install -y \
    git \
    zip \
    unzip \
    vim \
    nano \
    # install nodejs and npm
    && curl -sL https://deb.nodesource.com/setup_15.x | bash - \
    && apt-get install -y nodejs \
    # install yarn
    && apt-get install -y yarn \
    && apt-get install -y libpq-dev \
    && apt-get -y autoremove \
    && apt-get clean \
    && docker-php-ext-install pdo_mysql pdo_pgsql
WORKDIR /var/www/html
