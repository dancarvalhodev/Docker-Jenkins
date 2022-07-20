FROM jenkins/jenkins:lts

USER root

RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y && apt-get upgrade -y
RUN apt-get install -y -q build-essential curl nano