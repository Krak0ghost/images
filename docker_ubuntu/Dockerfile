FROM ubuntu

RUN apt update && apt upgrade -y

RUN apt install -y vim net-tools openssh-server 

CMD /usr/sbin/sshd -D

RUN apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common

RUN curl -fsSL https://download.docker.com/linux/ubuntu/gpg |  apt-key add -

RUN apt-key fingerprint 0EBFCD88

RUN add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

RUN apt update

RUN apt-get install -y docker-ce docker-ce-cli containerd.io

EXPOSE 22
EXPOSE 2377
