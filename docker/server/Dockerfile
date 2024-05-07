FROM php:8.3-apache
RUN a2enmod rewrite && \
curl -sSLf \
-o /usr/local/bin/install-php-extensions \
https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions && \
chmod +x /usr/local/bin/install-php-extensions && \
install-php-extensions gd pdo_mysql bcmath zip intl opcache @composer