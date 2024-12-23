# syntax=docker/dockerfile:1

# Comments are provided throughout this file to help you get started.
# If you need more help, visit the Dockerfile reference guide at
# https://docs.docker.com/go/dockerfile-reference/

# Want to help us make this template better? Share your feedback here: https://forms.gle/ybq9Krt8jtBL3iCk7

################################################################################

# Use JDK 21 image from the official OpenJDK registry
FROM openjdk:21-jdk

# Copy Hyperalloc to the working directory
WORKDIR /app
RUN ls -l /app
COPY target/HyperAlloc-1.0.jar hyperalloc.jar
RUN ls -l /app

#Specify how the application is to run
ENTRYPOINT ["java","-jar","hyperalloc.jar"]

