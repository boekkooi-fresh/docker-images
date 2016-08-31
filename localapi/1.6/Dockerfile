FROM node:slim

RUN apt-get update && apt-get install -y \
    git \
  && rm -rf /var/lib/apt/lists/*

ENV LOCALAPI_VERSION 1.6.0

RUN npm install --global "localapi@${LOCALAPI_VERSION}"

RUN mkdir -p /data
VOLUME /data
WORKDIR /data

ENTRYPOINT ["localapi"]

CMD ["--help"]
