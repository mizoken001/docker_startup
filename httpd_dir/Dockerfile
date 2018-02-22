# Dockerfile for Apache HTTP SErver

FROM enakai00/centos:centos6
MAINTAINER Toshiba Tarou

RUN echo "proxy=http://proxy.toshiba.co.jp:8080/" >> /etc/yum.conf
RUN echo "proxy=https://proxy.toshiba.co.jp:8080/" >> /etc/yum.conf
RUN yum -y install httpd
ADD index.html /var/www/html/index.html
CMD service httpd start && bash

