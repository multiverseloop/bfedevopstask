FROM wordpress:php7.2-apache
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug
RUN apt-get update
COPY ./stuff_that_you_want_to_add/ /var/www/html/