FROM ubuntu:24.04
RUN apt-get update
RUN apt-get install -y build-essential
ENV FILE_NAME=hello.c
VOLUME /app
WORKDIR /app
ENTRYPOINT gcc -o hello $FILE_NAME && ./hello