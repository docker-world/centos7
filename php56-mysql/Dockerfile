FROM dockerworld/centos7:php56

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="MySQL"

# install mysql
RUN yum install mysql -y
RUN yum install mysql-server -y
RUN chkconfig --level 345 mysqld on

EXPOSE 3306