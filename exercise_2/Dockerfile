# an image to compile and run java code in a container using openjdk-17-jdk
FROM openjdk:23-ea-17-jdk-bullseye
ENV FILE_NAME=main.java
VOLUME /app
WORKDIR /app
ENTRYPOINT javac $FILE_NAME && java Main