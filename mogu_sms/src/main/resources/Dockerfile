FROM openjdk:8-jre
MAINTAINER 1981196280@qq.com
ENV TZ=Asia/Shanghai
ENV LANG C.UTF-8
ENV NLS_LANG "SIMPLIFIED CHINESE"
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

EXPOSE 8604
ENV JAVA_OPT="-Xmx256m -Xms128m -Xmn256k"
ADD  mogu_sms-1.0.0.jar   app.jar
ENTRYPOINT java $JAVA_OPT -jar app.jar

