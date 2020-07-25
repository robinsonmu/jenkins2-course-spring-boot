FROM openjdk:8-jdk-alpine

LABEL maintaner="Robinson Munoz"
RUN ["rm", "-fr", "/usr/local/tomcat/webapps/*"]
ARG JAR_FILE=target/*.jar
# COPY path-to-your-application-war path-to-webapps-in-docker-tomcat
COPY ${JAR_FILE} /app.jar

EXPOSE 8080
ENTRYPOINT ["java","-jar","/app.jar"]


# CMD ["java", "-jar", "/app.jar"]
# docker build -t prueba .   
#  docker run -p 5001:8080 --name java prueba