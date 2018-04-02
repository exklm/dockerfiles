# Build with Ubuntu for easier time debugging
FROM ubuntu:16.04
MAINTAINER exklm@bitsgofer.com

ARG UBUNTU_MIRROR=archive.ubuntu.com
ARG VERSION=6.0.11

RUN sed -i -e "s/archive.ubuntu.com/$UBUNTU_MIRROR/g" /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y npm nodejs
RUN ln -s /usr/bin/nodejs /usr/bin/node
RUN npm install -g postcss@${VERSION} postcss-cli cssnano autoprefixer

ENTRYPOINT [ "postcss" ]
