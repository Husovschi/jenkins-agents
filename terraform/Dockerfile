FROM hashicorp/terraform:light as terraform
FROM jenkins/agent:alpine-jdk11 as jenkins

USER root

COPY --from=terraform /bin/terraform /usr/bin/terraform

USER jenkins