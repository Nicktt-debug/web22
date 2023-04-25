# Web server exemple hsix1
# Servidor apache interactiu
FROM debian:latest
LABEL  autor="Muhammad ahsan"
LABEL subject="webserver"
RUN apt-get update
RUN apt-get -y install vim nmap iproute2 procps net-tools xinetd telnet
RUN mkdir /opt/docker

COPY xinetd.d /etc/xinetd.d
COPY startup.sh /opt/docker

#CMD service xinetd start -dontfork && /bin/bash


RUN chmod +x /opt/docker/startup.sh

WORKDIR /opt/docker
CMD /opt/docker/startup.sh

#CMD /bin/bash

