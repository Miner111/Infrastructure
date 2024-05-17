FROM jenkins/ssh-agent:5.12.0-jdk17
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y curl git python3 python3-pip unzip ansible
RUN groupadd -g 997 docker && usermod -aG docker jenkins
RUN curl -fsSL https://get.docker.com/ | sh