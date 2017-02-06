# Ubuntu LTS based PHP-FPM

Make your own image with needed depencies like the Dockerfile:

```
FROM doigu/php-fpm

RUN apt-get update \
    && apt-get install -y php-memcache php7.0-gd php7.0-curl php7.0-json php7.0-mysql php7.0-readline php7.0-xml php7.0-xmlrpc php7.0-xsl php-geoip php7.0-mbstring \
    && rm -rf /var/lib/apt/lists/*
```
