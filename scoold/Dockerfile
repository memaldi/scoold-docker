FROM openjdk:8

RUN mkdir /src
WORKDIR /src

RUN wget https://github.com/memaldi/scoold/releases/download/1.28.2b/scoold-1.28.2.jar
COPY application.conf /src/application.conf

ENTRYPOINT ["java", "-jar", "-Dserver.port=8000", "-Dconfig.file=./application.conf", "scoold-1.28.0.jar"]
