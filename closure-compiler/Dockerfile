FROM ubuntu:16.04
MAINTAINER exklm@bitsgofer.com

ARG UBUNTU_MIRROR=archive.ubuntu.com
ARG VERSION=20160517.1.0

RUN sed -i -e "s/archive.ubuntu.com/$UBUNTU_MIRROR/g" /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y openjdk-9-jre nodejs npm
RUN npm install google-closure-compiler@${VERSION}

ENTRYPOINT [ "/usr/bin/java", "-jar", "/node_modules/google-closure-compiler/compiler.jar" ]
