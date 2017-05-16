# config-server
mvn package docker:build

docker run -p 8888:8888 -t nekperu15739/spring-cloud-config:latest

https://docs.docker.com/engine/userguide/eng-image/dockerfile_best-practices/#volume

If a service can run without privileges, use USER to change to a non-root user. Start by creating the user and group in the 
Dockerfile with something like RUN groupadd -r postgres && useradd -r -g postgres postgres