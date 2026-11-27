FROM serversideup/php:8.4-fpm-nginx
 
ARG HOST_UID=1000
ARG HOST_GID=1000
 
USER root
RUN docker-php-serversideup-set-id www-data ${HOST_UID}:${HOST_GID} && \
    docker-php-serversideup-set-file-permissions --owner ${HOST_UID}:${HOST_GID} --service nginx
USER www-data
 