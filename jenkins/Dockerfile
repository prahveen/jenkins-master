FROM jenkins/jenkins:lts

LABEL maintainer="Prahveen Thiruchelvam <prahveent@gmail.com>"

USER root

RUN apt-get update

USER jenkins

COPY plugins.txt /usr/share/jenkins/plugins.txt
COPY executors.groovy /usr/share/jenkins/ref/init.groovy.d/executors.groovy

RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/plugins.txt

RUN echo 2.0 > /usr/share/jenkins/ref/jenkins.install.UpgradeWizard.state


