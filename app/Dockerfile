# Use an official Maven/Java image as a parent image
FROM maven:3.8-openjdk-17-slim

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Build the Java application
RUN mvn clean install

# Make port 8080 available to the world outside this container
EXPOSE 8080

# Run app.jar when the container launches
CMD ["java", "-jar", "target/app.jar"]
