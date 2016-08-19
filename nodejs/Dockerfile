FROM node:6.4-wheezy

RUN apt-get update && apt-get install -y wget openjdk-7-jdk --fix-missing
RUN npm install -g pnpm selenium-standalone
RUN selenium-standalone install
