FROM ccr.ccs.tencentyun.com/devopsvip/dragonwell:21-anolis

WORKDIR /pig-register

ARG JAR_FILE=target/pig-register.jar

COPY ${JAR_FILE} app.jar

EXPOSE 8848 9848

ENV TZ=Asia/Shanghai JAVA_OPTS="-Xms128m -Xmx256m -Djava.security.egd=file:/dev/./urandom"

CMD sleep 30; java $JAVA_OPTS -jar app.jar
