# Use latest stable OpenJDK 11 (Eclipse Temurin)
FROM eclipse-temurin:11-jre-alpine

# Argument for JAR file
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy JAR file into container
COPY ${artifact} app.jar

# Expose application port (default Spring Boot port)
EXPOSE 8080

# Run the application
ENTRYPOINT ["java","-jar","app.jar"]
