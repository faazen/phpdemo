
FROM php:7.4.29
RUN  a2enmod rewrite

# Copy application source
ADD ./ /var/www/html
RUN chown -R www-data:www-data /var/www


FROM ubuntu/apache2
COPY 000-default.conf /etc/apache2/sites-available/000-default.conf
COPY apache2.conf /etc/apache2/apache2.conf
