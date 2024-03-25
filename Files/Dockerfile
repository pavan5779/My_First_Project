# Use an appropriate base image
FROM adoptopenjdk/openjdk11:alpine-jre

# Set the working directory
WORKDIR /opt/app

# Copy the JAR file into the container
COPY target/spring-boot-web.jar app.jar

# Expose the port that the Spring Boot application listens on
EXPOSE 8080

# Command to run the Spring Boot application
CMD ["java", "-cp", "app.jar", "com.example.demo.DemoApplication"]
