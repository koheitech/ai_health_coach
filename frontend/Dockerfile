FROM node:20

WORKDIR /app

ENV LANG C.UTF-8
ENV TZ Asia/Tokyo

RUN apt-get update -y && \
  apt-get upgrade -y && \
  npm install npm && \
  npm install nuxt && \
  npm install defu

ADD . /app