FROM jenkins/jenkins:latest-jdk25

USER root
RUN apt-get update && \
    apt-get install -y docker.io && \
    apt-get clean

RUN groupadd -f docker && usermod -aG docker jenkins

USER jenkins
