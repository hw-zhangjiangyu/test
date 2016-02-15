FROM reg.docker.alibaba-inc.com/alios6u2
MAINTAINER xijun.rxj <xijun.rxj@alibaba-inc.com>

#set yum config
#RUN rm -rf /etc/yum.repos.d/*
#COPY alios.repo /etc/yum.repos.d/

#install utilities
RUN yum -y install wget unzip gzip nmap telnet openssh-server.x86_64 openssh-clients perl-Data-Dumper-2.145-3.el7.x86_64 && echo "root:alios6u2" | chpasswd && service sshd start

#install alinpm & nvm
