
FROM php:7.4.29


# Copy application source



FROM ubuntu/apache2
ADD ./ /var/www/html
RUN chown -R www-data:www-data /var/www/html
COPY 000-default.conf /etc/apache2/sites-available/000-default.conf
COPY apache2.conf /etc/apache2/apache2.conf
RUN  service apache2 restart
