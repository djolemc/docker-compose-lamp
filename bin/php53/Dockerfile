FROM orsolin/docker-php-5.3-apache:latest


RUN apt-get update

#Midnight Commander
RUN apt-get install mc -y

# Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

EXPOSE 80

ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]