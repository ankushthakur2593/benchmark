FROM openjdk:11-jdk-slim

RUN apt-get update && \
    apt-get install -y curl && \
    rm -rf /var/lib/apt/lists/*

RUN curl -L -H 'Accept-Encoding: gzip' https://www.apache.org/dist/activemq/activemq-artemis/2.27.1/apache-artemis-2.27.1-bin.tar.gz -o apache-artemis-2.27.1-bin.tar.gz && tar -xzf apache-artemis-2.27.1-bin.tar.gz && rm apache-artemis-2.27.1-bin.tar.gz

WORKDIR /apache-artemis-2.27.1/bin