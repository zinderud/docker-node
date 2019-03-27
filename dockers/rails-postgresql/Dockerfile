FROM ruby:2.4.0
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
RUN mkdir /myapp
WORKDIR /myapp
COPY . /myapp
RUN bundle install

