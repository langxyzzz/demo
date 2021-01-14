#ARG repo
#FROM ${repo:-harbor.neusoft.com:8000}/library/openjdk:8-jdk-alpine

#EXPOSE 18081

#RUN mkdir -p /opt/sunpiaoliang/test-docker && mkdir -p /etc/sunpiaoliang
#ARG JAR_FILE
#COPY ${JAR_FILE} /opt/sunpiaoliang/test-docker/test-docker.jar
#ARG CONFIG_FILE
#COPY docker/config.conf /etc/sunpiaoliang/application.yml
#CMD ["java", "-Xmx1024m", "-Xms512m", "-Dspring.config.location=/etc/sunpiaoliang/application.yml", "-Dfile.encoding=UTF8", "-Duser.timezone=GMT+08", "-jar", "/opt/sunpiaoliang/test-docker/test-docker.jar"]

ARG repo
FROM openjdk:8-jdk-alpine
EXPOSE 9999
RUN mkdir -p /opt/langxy/test-docker && mkdir -p /etc/langxy
ARG JAR_FILE
COPY ${JAR_FILE} /opt/langxy/test-docker/test-docker.jar
CMD ["nohup", "java", "-Xmx1024m", "-Xms512m", "-Dfile.encoding=UTF8", "-Duser.timezone=GMT+08", "-jar", "/opt/langxy/test-docker/test-docker.jar"]