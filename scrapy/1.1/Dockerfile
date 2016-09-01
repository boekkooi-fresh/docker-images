FROM python:3.3-slim

ENV SCRAPY_VERSION ">=1.1,<1.2"

RUN python -m pip install "Scrapy${SCRAPY_VERSION}" Pillow
RUN mkdir -p /data
VOLUME /data
WORKDIR /data

ENTRYPOINT ["scrapy"]

CMD ["--help"]
