FROM node:slim

ENV ABAO_VERSION ^0.4.0-beta

RUN npm install --global "abao@${ABAO_VERSION}"

RUN mkdir -p /data
VOLUME /data
WORKDIR /data

ENTRYPOINT ["abao"]

CMD ["--help"]
