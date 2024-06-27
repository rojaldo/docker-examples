FROM ubuntu:24.04
RUN apt update
RUN apt install -y wget
ENV SERVER_URL=server:80/sample.html
VOLUME /app
WORKDIR /app
ENTRYPOINT wget $SERVER_URL