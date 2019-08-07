FROM ruby:2.5-alpine

RUN mkdir /app
WORKDIR /app

COPY Gemfile Gemfile.lock /app
RUN bundle install --jobs 4 --retry 3
COPY . .
