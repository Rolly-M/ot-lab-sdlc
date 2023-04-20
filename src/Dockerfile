# Set the base image
FROM tomcat:8.5.47-jdk8-openjdk

# Set the working directory
WORKDIR /usr/local/tomcat/webapps

# Copy built project to working directory 
COPY target/vprofile-v2.war .

# Expose the port that the Java app will listen on
EXPOSE 8080
