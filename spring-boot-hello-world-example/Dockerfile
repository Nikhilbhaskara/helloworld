# Start with a base image containing Java runtime
FROM openjdk:8      

# Add Maintainer Info
MAINTAINER = "Nikhil"

# Add a volume pointing to /tmp
VOLUME /tmp

# Make port 8080 available to the world outside this container
EXPOSE 8080

# The application's jar file
#ARG JAR_FILE=target/spring-boot-hello-world-example-0.0.1-SNAPSHOT.jar

# Add the application's jar to the container
 ADD /home/vsts/work/1/s/target/spring-boot-hello-world-example-0.0.1-SNAPSHOT.jar spring-boot-hello-world-example-0.0.1-SNAPSHOT.jar

#COPY /target/spring-boot-hello-world-example-0.0.1-SNAPSHOT.jar app.jar


# Run the jar file 
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
