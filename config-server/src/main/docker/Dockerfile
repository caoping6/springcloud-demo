FROM java:alpine
VOLUME /tmp
ENV PROFILE default
ENV JAVA_OPTS -server
ENTRYPOINT java -Dspring.profiles.active=${PROFILE} -Duser.timezone=Asia/Shanghai ${JAVA_OPTS} -jar /app.jar
EXPOSE 8761
ADD config-server-0.0.1-SNAPSHOT.jar /app.jar
