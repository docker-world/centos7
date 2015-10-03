FROM centos:7

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="Vim, Git"

# update
RUN yum update -y

# install vim
RUN yum install vim -y

# install git
RUN yum install git -y

# yum clean all
RUN yum clean all