FROM ruby:3.0

RUN mkdir /var/www
COPY main.rb /var/www
COPY Gemfile .

RUN gem update \
    && gem install bundler \
    && bundle install

CMD ["ruby", "/var/www/main.rb"]