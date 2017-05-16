FROM store/oracle/serverjre:8
RUN groupadd -r javagroup && useradd -r -g javagroup javauser
USER javauser
ADD /spring-cloud-config-0.0.1-SNAPSHOT.war /tmp/
ENTRYPOINT ["java", "-jar", "/tmp/spring-cloud-config-0.0.1-SNAPSHOT.war"]