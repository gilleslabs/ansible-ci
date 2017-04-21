# Latest Ubuntu LTS
FROM ubuntu:14.04
MAINTAINER Gilles Tosi
RUN apt-get update -y && \
apt-get install -y openssh-server && \
apt-get clean
RUN mkdir /var/run/sshd

RUN echo 'root:root' |chpasswd

RUN sed -ri 's/^PermitRootLogin\s+.*/PermitRootLogin yes/' /etc/ssh/sshd_config
RUN sed -ri 's/UsePAM yes/#UsePAM yes/g' /etc/ssh/sshd_config

EXPOSE 22

CMD    ["/usr/sbin/sshd", "-D"]
