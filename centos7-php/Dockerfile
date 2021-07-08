FROM centos:centos7.9.2009

LABEL maintainer="Kevin Bui"

RUN yum -y install epel-release \
    && yum -y update \
    && yum -y install httpd mod_ssl \
    && yum -y install php php-common php-fpm php-bcmath php-cli php-gd php-mbstring php-xml php-xmlrpc php-zip php-pgsql \
    && yum -y install unzip \
    && yum -y clean all
