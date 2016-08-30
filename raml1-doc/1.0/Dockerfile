FROM node:slim

ENV RAML1DOC_VERSION ^1.0.0

RUN npm install --global "raml1-doc@${RAML1DOC_VERSION}"

RUN mkdir -p /data
VOLUME /data
WORKDIR /data

ENTRYPOINT ["raml1-doc"]

CMD ["--help"]
