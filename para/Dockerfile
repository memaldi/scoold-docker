FROM openjdk:8

RUN mkdir /src
WORKDIR /src

RUN wget https://oss.sonatype.org/service/local/repositories/releases/content/com/erudika/para-war/1.28.0/para-war-1.28.0.war
COPY application.conf /src/application.conf

ENTRYPOINT ["java", "-jar", "-Dconfig.file=./application.conf", "para-war-1.28.0.war"]
