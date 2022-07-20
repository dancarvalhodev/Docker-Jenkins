FROM jenkins/jenkins:lts

USER root

RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y && apt-get upgrade -y
RUN apt-get install -y curl nano

RUN echo deb http://deb.debian.org/debian sid main contrib non-free >> /etc/apt/sources.list
RUN echo deb-src http://deb.debian.org/debian sid main contrib non-free >> /etc/apt/sources.list

RUN apt-get update && apt-get install -y gcc-12 build-essential -t sid