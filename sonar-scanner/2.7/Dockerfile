FROM java:8

ENV SONAR_SCANNER_VERSION 2.7

ADD "https://sonarsource.bintray.com/Distribution/sonar-scanner-cli/sonar-scanner-${SONAR_SCANNER_VERSION}.zip" /
RUN unzip "sonar-scanner-${SONAR_SCANNER_VERSION}.zip"

RUN mkdir -p /data
VOLUME /data
WORKDIR /data

ENV PATH "/sonar-scanner-${SONAR_SCANNER_VERSION}/bin:${PATH}"

ENTRYPOINT ["sonar-scanner"]

CMD ["--help"]
