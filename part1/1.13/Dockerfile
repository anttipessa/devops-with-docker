FROM openjdk:8-jdk-alpine

RUN apk add --no-cache maven

WORKDIR /java
COPY . /java

RUN ./mvnw package

EXPOSE 8080

CMD ["java" ,"-jar", "./target/docker-example-1.1.3.jar"]
