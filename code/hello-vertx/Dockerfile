FROM openjdk:8u131-jre

RUN apt-get update \
    && apt-get install -y \
       netcat  \
    && apt-get clean

EXPOSE 8080

COPY ./build/libs/my-service-0.0.1-SNAPSHOT.jar /var/my-service.jar

CMD ["java", "-jar", "/var/my-service.jar"]
