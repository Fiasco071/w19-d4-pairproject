FROM drupal:9.2.18-php7.4-apache-buster

RUN apt-get update && apt-get install -y git

RUN rm -rf /var/lib/apt/lists/*

WORKDIR /var/www/html/themes

RUN git clone --branch 8.x-3.x --single-branch --depth 1 https://git.drupal.org/project/bootstrap.git

RUN chown -R www-data:www-data bootstrap
