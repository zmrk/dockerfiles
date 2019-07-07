FROM       node:8
MAINTAINER hello@crazyguys.me

ENV        NODE_ENV="development"

RUN        ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime

WORKDIR    /root
ADD        server.tar ./

EXPOSE     3000
CMD        ["node", "server"]