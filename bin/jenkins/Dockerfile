FROM jenkinsci/blueocean:latest

RUN groupadd docker
RUN usermod -aG docker $USER
RUN chmod 777 /var/run/docker.sock