FROM jenkins
MAINTAINER Gilles Tosi
USER root
RUN apt-get update -y && \
apt-get install software-properties-common -y && \
apt-add-repository ppa:ansible/ansible -y && \
apt-get install ansible -y && \
apt-get install git -y && \
apt-get clean
USER jenkins

