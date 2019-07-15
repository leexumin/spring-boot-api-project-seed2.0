FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD spring-boot-api-project-seed.jar seed.jar
RUN sh -c 'touch /seed.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /seed.jar" ]