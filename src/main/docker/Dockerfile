FROM java:8u111-alpine
MAINTAINER whj1928@qq.com
VOLUME /var
ENV TZ="Asia/Shanghai" HOME="/var/app/"
WORKDIR ${HOME}
ADD eureka-server.jar /var/app/eureka-server.jar
EXPOSE 1111
ENTRYPOINT ["java" , "-Djava.security.egd=file:/dev/./urandom", "-jar" ,"/var/app/eureka-server.jar"]