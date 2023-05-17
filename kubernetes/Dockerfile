FROM alpine/helm as helm
FROM jenkins/agent:jdk11 as jenkins

USER root

COPY --from=helm /usr/bin/helm /usr/bin/helm
RUN apt-get update && apt-get install -y python3.9

USER jenkins