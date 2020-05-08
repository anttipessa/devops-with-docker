FROM ruby:2.6.0

RUN bundle config --global frozen 1
RUN apt-get update -qq && apt-get install -y nodejs

WORKDIR /usr/bin/app

COPY Gemfile Gemfile.lock ./
RUN bundle install
COPY . .

EXPOSE 3000

RUN rails db:migrate

CMD ["rails", "s" ]
