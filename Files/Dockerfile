# Use an appropriate base image
FROM adoptopenjdk/openjdk11:alpine-jre

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# Debug: List contents of the JAR file
RUN jar tf app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
