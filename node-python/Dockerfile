FROM python

RUN apt-get update \
  && apt-get install -y sudo \
  && curl -fsSL https://deb.nodesource.com/setup_15.x | sudo -E bash - \
  && sudo apt-get install -y nodejs \
  && npm install --global npm \
  && npm install --global yarn

CMD [ "node" ]