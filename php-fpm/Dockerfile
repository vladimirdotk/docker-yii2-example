FROM phpdockerio/php71-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php7.1-mysql php-redis php7.1-sqlite3 php7.1-bcmath php7.1-bz2 php7.1-gd php7.1-imap php-imagick php7.1-mbstring php-yaml php-xdebug \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


WORKDIR "/var/www/docker-yii2-example"