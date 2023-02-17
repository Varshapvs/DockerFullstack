FROM openjdk:17-jdk-slim-buster

WORKDIR /Springboot
COPY . .
RUN gradlew.bat clean build

VOLUME /tmp
EXPOSE 8081
ADD /build/libs/demo-0.0.1-SNAPSHOT.jar demo-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java","-jar","demo-0.0.1-SNAPSHOT.jar"]

