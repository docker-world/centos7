FROM dockerworld/centos7:base

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="Httpd"

RUN yum install httpd -y
RUN systemctl enable httpd
RUN perl -pi -e "s/;EnableSendfile Off/EnableSendfile Off/g" /etc/httpd/conf/httpd.conf
RUN yum clean all

EXPOSE 80
EXPOSE 443