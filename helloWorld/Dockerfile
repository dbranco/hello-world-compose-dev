FROM openjdk:11
WORKDIR /java/src/github.com/com/test
COPY . .

RUN ./gradlew build
CMD ["./gradlew", "bootRun"]