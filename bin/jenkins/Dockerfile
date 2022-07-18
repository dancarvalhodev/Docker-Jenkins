FROM devopsjourney1/myjenkinsagents:python

USER root

# Essentials
RUN echo "UTC" > /etc/timezone
RUN apk add --no-cache zip unzip curl

# Installing bash
RUN apk add bash
RUN sed -i 's/bin\/ash/bin\/bash/g' /etc/passwd

RUN apk add --no-cache php8 \
    php8-common \
    php8-pdo \
    php8-opcache \
    php8-zip \
    php8-phar \
    php8-iconv \
    php8-cli \
    php8-curl \
    php8-openssl \
    php8-mbstring \
    php8-tokenizer \
    php8-fileinfo \
    php8-json \
    php8-xml \
    php8-xmlwriter \
    php8-simplexml \
    php8-dom \
    php8-pdo_mysql \
    php8-tokenizer