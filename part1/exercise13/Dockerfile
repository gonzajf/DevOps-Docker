FROM openjdk:8
WORKDIR /exercise13
COPY spring-example-project-master /exercise13
RUN ./mvnw package
EXPOSE 8080
CMD ["java","-jar","./target/docker-example-1.1.3.jar"]