# Build the project using Maven
FROM maven:3.8.6-eclipse-temurin-8-alpine AS maven
LABEL MAINTAINER="iamkoldzo@gmail.com"

RUN apk update
RUN apk add git

RUN git clone https://github.com/kkenan/basic-microservices.git

RUN mv basic-microservices/spring-boot-app /spring-boot-app
RUN rm -r basic-microservices/

WORKDIR /spring-boot-app

RUN mvn clean package
RUN cp target/*.jar app.jar

# Run the project
FROM openjdk:8-jdk-alpine
ARG JAR_FILE=app.jar

COPY my-conf.yml /opt/app/application.yml
COPY --from=maven /spring-boot-app/${JAR_FILE} /opt/app/
WORKDIR /opt/app

EXPOSE 8080

ENTRYPOINT ["java","-jar", "app.jar", "--spring.config.location=application.yml"]
