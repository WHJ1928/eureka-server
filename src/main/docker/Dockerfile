#指定基础镜像
FROM java:8u111-alpine
#指定作者
MAINTAINER whj1928@qq.com
#将文件夹挂载到容器中
VOLUME /var
#将文件复制到镜像中
ADD eureka.jar /var/app/eureka.jar
#设置环境变量
ENV TZ="Asia/Shanghai" HOME="/var/app/"
#设置工作目录
WORKDIR ${HOME}
#指定暴露的端口
EXPOSE 6666
#启动时的默认命令
ENTRYPOINT ["java" , "-Djava.security.egd=file:/dev/./urandom", "-jar" ,"/var/app/eureka.jar"]