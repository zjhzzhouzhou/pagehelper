FROM openjdk:8-jre-alpine

MAINTAINER zhouzhou
LABEL name="pagehelper-demo" version="1.0" author="zhouzhou"

ENV SERVICE_NAME pagehelper
ENV OPS "--spring.profiles.active=test -server -Xms256m -Xmx256m -Xss256k"

RUN mkdir -p /data/logs
ADD ${SERVICE_NAME}-0.0.1-SNAPSHOT.jar ${SERVICE_NAME}-image.jar
ENTRYPOINT java -jar ${OPS} ${SERVICE_NAME}-image.jar

