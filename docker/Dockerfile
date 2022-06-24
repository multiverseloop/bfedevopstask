FROM wordpress:latest
RUN apt-get update && \
    apt-get -y install vim

RUN pecl install xdebug  \
    && docker-php-ext-enable xdebug


ADD ./php.ini /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini

COPY ./stuff_that_you_want_to_add/ /var/www/html/