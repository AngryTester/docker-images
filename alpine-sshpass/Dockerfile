FROM alpine:3.5

MAINTAINER AngryTester <thx_phila@yahoo.com>

ENV LANG=C.UTF-8

RUN apk add --no-cache tzdata && \
    cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone && \
    apk del tzdata

RUN apk add --no-cache openssh sshpass
    
RUN echo "StrictHostKeyChecking no">>/etc/ssh/ssh_config
