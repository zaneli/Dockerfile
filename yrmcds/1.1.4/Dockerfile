FROM centos:7

MAINTAINER Shunsuke Otani <shun.otani@gmail.com>

RUN yum install -y make wget gcc-c++ libatomic.x86_64

RUN cd /root/ && wget https://github.com/cybozu/yrmcds/archive/v1.1.4.tar.gz
RUN cd /root/ && tar xfz v1.1.4.tar.gz

RUN groupadd nogroup

RUN mkdir -m 755 /var/tmp/yrmcds
RUN mkdir -m 755 /etc/init/

RUN cd /root/yrmcds-1.1.4/ && make
RUN cd /root/yrmcds-1.1.4/ && make install

EXPOSE 11211

ENTRYPOINT ["/usr/local/sbin/yrmcdsd"]
