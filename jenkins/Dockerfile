FROM jenkins/jenkins:2.277.4-lts-jdk11
USER root
RUN apt-get update && apt-get install -y apt-transport-https \
       ca-certificates curl gnupg2 \
       software-properties-common
USER jenkins
RUN jenkins-plugin-cli --plugins "blueocean:1.24.6 prometheus:2.0.10 "
EXPOSE 8080
EXPOSE 50001