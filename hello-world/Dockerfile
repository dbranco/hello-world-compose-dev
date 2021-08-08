FROM openjdk:11 AS build
FROM build AS development

WORKDIR /src
COPY . .

#FROM registry.jetbrains.team/p/prj/containers/projector-idea-u AS development
# RUN apt-get update \
#     && apt-get install -y git
CMD ["./gradlew", "bootRun"]