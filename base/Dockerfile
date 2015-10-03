FROM centos:7

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="Dockerfile to build CentOS 7 container images:\
Vim\
Git"

# update
RUN yum update -y

# vim
RUN yum install vim -y

# git
RUN yum install git -y

# clean all
RUN yum clean all