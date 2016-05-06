FROM alpine:3.3

MAINTAINER Shunsuke Otani <shun.otani@gmail.com>

RUN apk --no-cache add openjdk8 bash
ENV JAVA_HOME /usr/lib/jvm/default-jvm/

RUN cd /root/ && wget https://github.com/Frege/frege-repl/releases/download/1.2.1-SNAPSHOT/fregei-1.2.1-SNAPSHOT.zip
RUN cd /root/ && unzip fregei-1.2.1-SNAPSHOT.zip

ENTRYPOINT ["/root/fregei-1.2.1-SNAPSHOT/bin/fregei"]
