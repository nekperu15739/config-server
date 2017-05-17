# config-server
* [Overview](URL "overview")
* [Build](URL "Build")
* [Run](URL "Run")
* [Image Repository](URL "Image Repository")
* [Backoffice](URL "Backoffice")

## Overview
This project it's a sample implementation of **spring cloud config server**, using Spring-Cloud stack with Java 8, more information will be found here: http://cloud.spring.io/spring-cloud-config/

```java

@EnableConfigServer
@SpringBootApplication
public class ConfigServerApplication {

	public static void main(String[] args) {
		SpringApplication.run(ConfigServerApplication.class, args);
	}
}

``

## Build
mvn package docker:build

## Run
docker run -p 8888:8888 -t nekperu15739/spring-cloud-config:latest

## Image Repository
The lastest image is public here: https://hub.docker.com/r/nekperu15739/spring-cloud-config/

## Backoffice
The backoffice throw config server it's obviously git, and on this case the resources to public are in https://github.com/nekperu15739/config-repo
