# Latest Ubuntu LTS
FROM ubuntu:14.04
MAINTAINER Gilles Tosi
RUN apt-get update -y && \
apt-get install software-properties-common -y && \
apt-add-repository ppa:ansible/ansible -y && \
apt-get install ansible -y && \
apt-get install sshpass -y && \
apt-get install rsync -y && \
apt-get install curl -y && \
apt-get clean

