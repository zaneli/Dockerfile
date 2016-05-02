FROM centos:7

MAINTAINER Shunsuke Otani <shun.otani@gmail.com>

RUN yum install -y wget unzip java-1.8.0-openjdk

RUN localedef -vc -i en_US -f UTF-8 en_US.UTF-8 | true
ENV LANG en_US.UTF-8
ENV JAVA_HOME /usr/lib/jvm/java-1.8.0-openjdk-1.8.0.91-0.b14.el7_2.x86_64/jre/

RUN cd /root/ && wget https://github.com/Frege/frege-repl/releases/download/1.2.1-SNAPSHOT/fregei-1.2.1-SNAPSHOT.zip
RUN cd /root/ && unzip fregei-1.2.1-SNAPSHOT.zip

ENTRYPOINT ["/root/fregei-1.2.1-SNAPSHOT/bin/fregei"]
