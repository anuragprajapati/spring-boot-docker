# spring-boot-dockerize
How to Dockerize Spring Boot Application 

# Build Docker Image 
$ docker build -t spring-boot-docker.jar .

# Check Docker Image 
$ docker image ls

# Run Docker Image 
$ docker run -p 9090:8080 spring-boot-docker.jar

In the run command, we have specified that the port 8080 on the container should be mapped to the port 9090 on the Host OS.

#Docker verious commands

$ docker -v ==> for showing version of the docker

$ docker build -t spring-boot-docker.jar => for building the docker image

$ docker image ls  => for seeing the docker image

$ docker run -p 9090:8080 spring-boot-docker.jar  => for running the application using docker image 9090=> port no. is for docker and 8080 for the tomcat

$ docker login => for login into the docker hub

$ docker tag spring-boot-docker.jar code2java/spring-boot-docker.jar => for adding the tag name as code2java, because docker hub is the public hosted repository, and we need to give unique tag name to identify our repository;

$ docker push code2java/spring-boot-docker.jar => for pushing the docker image into the docker hub

$ docker pull code2java/spring-boot-docker.jar => for pulling the docker image from the docker hub
