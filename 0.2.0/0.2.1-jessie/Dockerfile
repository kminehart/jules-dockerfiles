FROM debian:jessie-slim
MAINTAINER Kevin Minehart <kmineh0151@gmail.com>

RUN echo "deb http://ftp.debian.org/debian jessie-backports main" >> /etc/apt/sources.list

RUN apt-get update -yqqqq
RUN apt-get install -yqqqq curl golang-1.7 npm 
RUN apt-get autoremove -y
RUN apt-get clean -y

# Install some things people will probably use
RUN curl -sL https://github.com/kminehart/jules/releases/download/v0.2.1/jules > /bin/jules                                                                                           


RUN chmod +x /bin/jules

