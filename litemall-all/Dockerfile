FROM java:8-jre

ENV TZ=Asia/Shanghai

RUN ln -sf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

EXPOSE 8080

ADD ./target/litemall-all-0.1.0-exec.jar ./

CMD java -Djava.security.egd=file:/dev/./urandom -jar litemall-all-0.1.0-exec.jar