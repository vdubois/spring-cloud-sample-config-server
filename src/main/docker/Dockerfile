FROM frolvlad/alpine-oraclejdk8:slim
MAINTAINER Vincent Dubois <dubois.vct@free.fr>

VOLUME /tmp
ADD spring-cloud-sample-config-server-0.0.1-SNAPSHOT.jar app.jar
RUN sh -c 'touch /app.jar'
EXPOSE 9000
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]