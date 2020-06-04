FROM php:7.3.13-fpm-alpine3.10 as base

MAINTAINER Amir Ghaffari Heravi <contact@amirghaffari.com>

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/bin/

RUN install-php-extensions \
	    amqp \
	    apcu \
	    bcmath \
	    bz2 \
	    calendar \
	    cmark \
	    dba \
	    decimal \
	    enchant \
	    exif \
	    gd \
	    gettext \
	    gmagick \
	    gmp \
	    grpc \
	    http \
	    igbinary \
	    imagick \
	    imap \
	    interbase \
	    intl \
	    ldap \
	    mailparse \
	    mcrypt \
	    memcache \
	    memcached \
	    mongo \
	    mongodb \
	    msgpack \
	    mysqli \
	    oauth \
	    odbc \
	    opcache \
	    opencensus \
	    parallel \
	    pcntl \
	    pcov \
	    pdo_dblib \
	    pdo_firebird \
	    pdo_mysql \
	    pdo_odbc \
	    pdo_pgsql \
	    pdo_sqlsrv \
	    pgsql \
	    propro \
	    protobuf \
	    pspell \
	    raphf \
	    rdkafka \
	    recode \
	    redis \
	    shmop \
	    snmp \
	    snuffleupagus \
	    soap \
	    sockets \
	    solr \
	    sqlsrv \
	    ssh2 \
	    sysvmsg \
	    sysvsem \
	    sysvshm \
	    tdlib \
	    tidy \
	    timezonedb \
	    uopz \
	    uuid \
	    wddx \
	    xdebug \
	    xhprof \
	    xmlrpc \
	    xsl \
	    yaml \
	    zip

COPY --from=composer:2 /usr/bin/composer /usr/bin/composer

