# Use the official Eclipse Temurin image (successor to AdoptOpenJDK)
FROM eclipse-temurin:11-jre

# Artifact path from build
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the built jar
COPY ${artifact} app.jar

# Default entrypoint
ENTRYPOINT ["java", "-jar", "app.jar"]
