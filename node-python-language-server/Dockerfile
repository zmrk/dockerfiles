FROM       crazyguys/node-python

ENV        PYTHONPATH="${PYTHONPATH}:/root/python/lib"
ENV        NODE_ENV="development"

RUN        ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime && \
           mkdir -p /root/python/lib && \
           pip3 install python-language-server

WORKDIR    /root
ADD        server.tar ./

EXPOSE     3000
CMD        ["node", "server"]
