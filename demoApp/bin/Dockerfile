# Use a lightweight JRE 17 image (best for running, not building)
FROM eclipse-temurin:17-jre-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy the JAR file from your target folder to the container
# Replace 'demoApp-0.0.1-SNAPSHOT.jar' with your actual JAR name if different
COPY target/demoApp-0.0.1-SNAPSHOT.jar app.jar

# Inform Docker that the app listens on port 8080 (standard Spring default)
EXPOSE 8080

# Execute the application
ENTRYPOINT ["java", "-jar", "app.jar"]
