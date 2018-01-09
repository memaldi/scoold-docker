FROM openjdk:8

RUN mkdir /src
WORKDIR /src

RUN wget https://github.com/Erudika/scoold/releases/download/1.28.2/scoold-1.28.2.jar
COPY application.conf /src/application.conf

ENTRYPOINT ["java", "-jar", "-Dserver.port=8000", "-Dconfig.file=./application.conf", "scoold-1.28.2.jar"]
