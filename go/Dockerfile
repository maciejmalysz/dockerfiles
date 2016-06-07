FROM jdeathe/centos-ssh:centos-6
MAINTAINER Maciej Malysz <mmalysz@cisco.com>
ADD gocd.repo etc/yum.repos.d/gocd.repo
RUN yum install -y java-1.7.0-openjdk
RUN yum install -y go-server
RUN yum install -y go-agent
COPY go-generic-artifactory-poller.jar /tmp/go-generic-artifactory-poller.jar
RUN /etc/init.d/go-server start
RUN cp /tmp/go-generic-artifactory-poller.jar /var/lib/go-server/plugins/go-generic-artifactory-poller.jar
