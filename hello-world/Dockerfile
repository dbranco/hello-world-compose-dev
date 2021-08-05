FROM openjdk:11 AS build
WORKDIR /java/src/github.com/com/test
COPY . .

RUN ./gradlew build

FROM build AS development
RUN apt-get update \
    && apt-get install -y git
CMD ["./gradlew", "bootRun"]