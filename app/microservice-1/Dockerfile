# Use a base Java image
FROM openjdk:17.0.2-slim-buster

# Create directory for app
WORKDIR /app

# Copy the build artifact (JAR file) from the host machine into the Docker container
COPY app/microservice-1/build/libs/hello-springboot-0.0.1-SNAPSHOT.jar /app/app.jar

# Expose port 8080 (or whatever port your Spring Boot app uses)
EXPOSE 8080

# Command to run the app
ENTRYPOINT ["java", "-jar", "app.jar"]
