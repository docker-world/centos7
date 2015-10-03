FROM dockerworld/centos7:base

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="Httpd; \
PHP: 5.6 (PDO, MySQLI, XML, Intl), \
Composer"

# install httpd
RUN yum install httpd -y

# install php 5.6
RUN rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
RUN rpm -Uvh https://mirror.webtatic.com/yum/el7/webtatic-release.rpm
RUN yum install php56w php56w-opcache -y

# install php 5.6 extensions
RUN yum install php56w-pdo -y
RUN yum install php56w-mysqli -y
RUN yum install php56w-xml -y
sudo yum install php56w-intl -y

# set php date timezone
RUN perl -pi -e "s#;date.timezone =.*#date.timezone = Europe/London#g" /etc/php.ini

# yum clean all
RUN yum clean all

EXPOSE 80
EXPOSE 443