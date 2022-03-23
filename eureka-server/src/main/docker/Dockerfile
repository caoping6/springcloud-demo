FROM java:alpine
VOLUME /tmp
ENV PROFILE default
ENV JAVA_OPTS -server
ENTRYPOINT java -Dspring.profiles.active=${PROFILE} -Duser.timezone=Asia/Shanghai ${JAVA_OPTS} -jar /app.jar
EXPOSE 8761
ADD eureka-server-1.0-SNAPSHOT.jar /app.jar
