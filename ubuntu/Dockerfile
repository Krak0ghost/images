fROM ubuntu

RUN apt update && apt upgrade -y 

RUN apt install -y vim net-tools openssh-server
RUN service ssh start

CMD /usr/sbin/sshd -D

EXPOSE 22
