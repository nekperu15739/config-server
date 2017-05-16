FROM frolvlad/alpine-oraclejdk8:slim
ADD /spring-cloud-config-0.0.1-SNAPSHOT.war /tmp/
ENTRYPOINT ["java", "-jar", "/tmp/spring-cloud-config-0.0.1-SNAPSHOT.war"]