FROM openjdk:17-alpine
VOLUME /tmp
ARG JAR_FILE
COPY ./apps/${JAR_FILE}.jar app.jar
ENTRYPOINT ["java", "-XX:MaxRAMPercentage=75.0", "-Xmx1024M", "-jar", "/app.jar"]