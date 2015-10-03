############################################################
# Dockerfile to build CentOS 7 container images
# Based on CentOS 7
# Install: Vim, Git
############################################################

FROM centos:7
MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

# update
RUN yum update -y

# vim
RUN yum install vim -y

# git
RUN yum install git -y

# clean all
RUN yum clean all