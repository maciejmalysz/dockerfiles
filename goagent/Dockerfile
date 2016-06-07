# this Docker file is creating image for go agent with autoregistration to go server
# Install the Java
FROM jdeathe/centos-ssh:centos-6
MAINTAINER Maciej Malysz <mmalysz@cisco.com>
ADD gocd.repo etc/yum.repos.d/gocd.repo
RUN yum install -y java-1.7.0-openjdk
RUN yum install -y go-agent
