FROM centos:latest
MAINTAINER jiangyu.zjy <jiangyu.zjy@alibaba-inc.com>

#set yum config
#RUN rm -rf /etc/yum.repos.d/*
#COPY alios.repo /etc/yum.repos.d/

#install utilities
#RUN yum -y install wget unzip gzip nmap telnet openssh-server.x86_64 openssh-clients perl-Data-Dumper-2.145-3.el7.x86_64 && echo #"root:alios6u2" | chpasswd && service sshd start

ADD ./JDK /home/admin/jdk
ADD ./TOMCAT /home/admin/tomcat
ENV HAVA_HOME /home/admin/jdk
ENV CATALINA_HOME /home/admin/tomcat

EXPOSE 8080 12200 12201 8006 8005

CMD $CATALINA_HOME/bin/catalina.sh run

#install alinpm & nvm
