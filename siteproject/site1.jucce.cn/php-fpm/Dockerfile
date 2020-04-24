FROM php:7.3-fpm

ARG PUID=1000

ENV PUID ${PUID}

ARG PGID=1000

ENV PGID ${PGID}

RUN groupmod -o -g ${PGID} www-data && \
    usermod -o -u ${PUID} -g www-data www-data

EXPOSE 9000

WORKDIR /var/www

CMD ["php-fpm"]
