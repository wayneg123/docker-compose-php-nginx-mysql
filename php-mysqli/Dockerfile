FROM php:7.2-fpm

RUN apt-get update \
	&& sed -i 's/deb.debian.org/mirrors.ustc.edu.cn/g' /etc/apt/sources.list \
	&& apt-get install iputils-ping -y\
	&& docker-php-ext-install mysqli && docker-php-ext-enable mysqli
