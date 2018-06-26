FROM java:8u111-alpine
MAINTAINER whj1928@qq.com
VOLUME /var
ADD stat /var/lib/docker/tmp/docker-builder625808573/eureka-server.jar /var/app/eureka-server.jar
ENV TZ="Asia/Shanghai" HOME="/var/app/"
WORKDIR ${HOME}
EXPOSE 1111
ENTRYPOINT ["java" , "-Djava.security.egd=file:/dev/./urandom", "-jar" ,"/var/app/eureka-server.jar"]