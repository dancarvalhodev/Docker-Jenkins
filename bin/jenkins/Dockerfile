FROM jenkins/jenkins:lts

USER root

RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y && apt-get upgrade -y
RUN apt-get install -y curl nano
RUN apt-get install apt-transport-https ca-certificates curl gnupg2 software-properties-common
RUN curl -fsSL https://download.docker.com/linux/debian/gpg | apt-key add -
RUN add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian $(lsb_release -cs) stable"
RUN apt-get update && apt-install docker-ce

#RUN echo deb http://deb.debian.org/debian sid main contrib non-free >> /etc/apt/sources.list
#RUN echo deb-src http://deb.debian.org/debian sid main contrib non-free >> /etc/apt/sources.list
#
#RUN apt-get update && apt-get install -y gcc-12 build-essential -t sid