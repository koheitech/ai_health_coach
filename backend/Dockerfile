FROM ruby:3.2.3

ENV LANG C.UTF-8
ENV TZ Asia/Tokyo

RUN mkdir /app
WORKDIR /app

ADD Gemfile /app/Gemfile

RUN apt-get update -qq && \
  apt-get install -y build-essential \
  libpq-dev \
  sudo \
  gem install bundler -v 2.5.6

RUN bundle install

ADD . /app