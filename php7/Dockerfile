FROM alpine:edge

MAINTAINER Luca Corbo <lu.corbo@gmail.com>

WORKDIR /app

CMD ["php", "-a"]

RUN apk --no-cache --repository http://dl-cdn.alpinelinux.org/alpine/edge/testing  add \
        bash \
        ca-certificates \
        git \
        curl \
        unzip \
        php7 \
        php7-xml \
        php7-zip \
        php7-xmlreader \
        php7-zlib \
        php7-opcache \
        php7-mcrypt \
        php7-openssl \
        php7-curl \
        php7-json \
        php7-dom \
        php7-phar \
        php7-mbstring

RUN ln -s /usr/bin/php7 /usr/bin/php

COPY resources/php.ini /etc/php7/php.ini

