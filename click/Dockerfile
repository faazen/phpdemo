
FROM php:7.4-apache

COPY 000-default.conf /etc/apache2/sites-available/000-default.conf
COPY apache2.conf /etc/apache2/apache2.conf
RUN  a2enmod rewrite

# Copy application source
ADD ./ /var/www/html
RUN chown -R www-data:www-data /var/www
CMD ["apache2 -D FOREGROUND"]

