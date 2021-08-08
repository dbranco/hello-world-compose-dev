

#FROM openjdk:11 AS build
FROM registry.jetbrains.team/p/prj/containers/projector-idea-u AS build
WORKDIR /java/src/github.com/com/test
COPY . .

RUN ./gradlew build

FROM build AS development
#RUN apt-get update \
#    && apt-get install -y git
#CMD ["./gradlew", "bootRun"]
EXPOSE 8787

#FROM registry.jetbrains.team/p/prj/containers/projector-idea-u AS development
# RUN apt-get update \
#     && apt-get install -y git
