FROM node:slim

ENV LOCALAPI_VERSION 1.6.0

RUN npm install --global "localapi@${LOCALAPI_VERSION}"

RUN mkdir -p /data
VOLUME /data
WORKDIR /data

ENTRYPOINT ["localapi"]

CMD ["--help"]
