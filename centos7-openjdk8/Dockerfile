FROM centos:centos7.9.2009

LABEL maintainer="Kevin Bui"

RUN yum -y install epel-release \
    && yum -y update \
    && yum -y install java-1.8.0-openjdk java-1.8.0-openjdk-devel \
    && yum -y install unzip \
    && yum -y clean all

ENV JAVA_HOME /usr/lib/jvm/java-1.8.0-openjdk
