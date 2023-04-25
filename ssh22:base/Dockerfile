# Web server exemple hsix1
# Servidor apache interactiu
FROM debian:latest
LABEL  autor="Muhammad ahsan"
LABEL subject="SSH SERVER"
RUN apt-get update
RUN apt-get -y install procps iproute2 nmap tree vim  openssh-server openssh-client
RUN mkdir /opt/docker
COPY * /opt/docker
RUN chmod +x /opt/docker/startup.sh
WORKDIR /opt/docker
CMD /opt/docker/startup.sh
EXPOSE 22
