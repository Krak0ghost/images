FROM ubuntu

RUN apt update && apt upgrade -y

RUN apt install -y vim net-tools openssh-server 

RUN apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common iptables lxc

RUN curl -fsSL https://download.docker.com/linux/ubuntu/gpg |  apt-key add -

RUN apt-key fingerprint 0EBFCD88

RUN add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

RUN apt update

RUN apt-get install -y docker-ce

VOLUME /var/lib/docker
