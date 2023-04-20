FROM openjdk:latest

WORKDIR /usr/src/app

ENV POSTREGS_USER=kodilla

ENV POSTGRES_PASSWORD=kodilla

COPY . .

RUN microdnf install findutils

RUN ./gradlew build

EXPOSE 8080

CMD java -jar build/libs/quotes-0.0.1-SNAPSHOT.jar