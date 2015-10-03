FROM dockerworld/centos:stable
MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

RUN yum update && yum install httpd -y && yum clean

EXPOSE 80
EXPOSE 443


FROM dockerworld/centos7:base

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="Httpd"

# update
RUN yum install httpd -y

# clean all
RUN yum clean all

EXPOSE 80
EXPOSE 443