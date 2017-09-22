FROM openjdk:8-jre-alpine
ENV APP_DIR /usr/share/app
RUN adduser -D java
RUN mkdir -p $APP_DIR && chown -R java $APP_DIR
USER java
COPY config-server-0.0.1-SNAPSHOT.jar $APP_DIR/config-server-0.0.1-SNAPSHOT.jar
CMD java -jar $APP_DIR/config-server.jar