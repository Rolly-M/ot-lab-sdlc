# Set the base image to OpenJDK 11
FROM openjdk:11

# Install Git
RUN apt-get update && apt-get install -y git

# Clone the Java project from GitHub
RUN git clone https://github.com/username/repo.git /app

# Set the working directory
WORKDIR /app

# Build the Java project using Maven (or Gradle if your project uses that instead)
RUN ./mvnw clean package

# Expose the port that the Java app will listen on
EXPOSE 8080

# Start the Java app when the container starts
CMD ["java", "-jar", "/app/target/myapp.jar"]