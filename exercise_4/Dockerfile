FROM ubuntu:24.04
RUN apt-get update
RUN apt-get install -y openjdk-17-jdk git maven
ENV REPO=https://github.com/rojaldo/sprinboot3.git

# Clone the repository
USER root
CMD git clone $REPO springboot3 && cd springboot3 && chmod +x ./mvnw && ./mvnw clean package spring-boot:repackage && java -jar target/demo-0.0.1-SNAPSHOT.jar