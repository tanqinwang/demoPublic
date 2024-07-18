# FROM php:7.4-fpm as min

# # Install system packages
# RUN apt-get update && \
#     apt-get -y install \
#             nginx-full \
#             git \
#             unzip \
#         --no-install-recommends && \
#         apt-get clean && \
#         rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*


# COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/

# ARG EXTENTIONS="gd opcache bcmath calendar pcntl mysqli pdo_mysql sockets soap readline shmop xmlrpc zip redis @composer"
# RUN install-php-extensions $EXTENTIONS

# EXPOSE 80 443

FROM tanqinwang/nginx-php-fpm-base:latest
EXPOSE 80 443
