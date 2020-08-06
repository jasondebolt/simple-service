# Maven Spring Boot WebSocket app

A dockerized clone of the spring.io WebSocket example.

## Original Spring.io Guide
* [Spring.io WebSocket Guide](https://github.com/spring-guides/gs-messaging-stomp-websocket)
* [Spring.io WebSocket Git Repo](https://spring.io/guides/gs/messaging-stomp-websocket)

## Development Workflow
```$xslt
$ mvn spring-boot:run

Build project in intellij to redeploy
```

## Create a JAR
```$xslt
mvn clean package
```

## Build Docker Image
- Create a JAR, then run:
```$xslt
docker build -t web-sockets .
docker run -p 8080:8080 web-sockets
```
