# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM eclipse-temurin:17-jdk-alpine
LABEL authors="needhi"

# Simply the artifact path
ARG artifact=out/artifacts/springapp_jar/springapp.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

EXPOSE 8080
# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]