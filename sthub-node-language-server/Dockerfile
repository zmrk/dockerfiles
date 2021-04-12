FROM crazyguys/node-python

ENV PYTHONPATH="${PYTHONPATH}:/root/python/lib"
ENV NODE_ENV="development"

WORKDIR /root
COPY *.py ./python/lib/
COPY requirements.txt ./

RUN ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime \
  && mkdir -p /root/python/lib \
  && pip install python-language-server \
  && pip install -r requirements.txt

CMD ["node"]
