FROM tomcat:8.0-jre8

LABEL maintaner="Robinson Munoz"
RUN ["rm", "-fr", "/usr/local/tomcat/webapps/ROOT"]
# COPY path-to-your-application-war path-to-webapps-in-docker-tomcat
COPY ./target/spring-boot-sample-atmosphere-1.4.0.RELEASE.jar /usr/local/tomcat/webapps/

EXPOSE 8080

CMD ["catalina.sh", "run"]

# docker build -t prueba .   
#  docker run -p 5001:8080 --name java prueba