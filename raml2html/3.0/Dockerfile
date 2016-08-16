FROM node:slim

ENV RAML2HTML_VERSION 3.0.x

RUN npm install --global "raml2html@${RAML2HTML_VERSION}"

RUN mkdir -p /data
VOLUME /data
WORKDIR /data

ENTRYPOINT ["raml2yaml"]

CMD ["--help"]
