FROM ruby:2.6.0

WORKDIR /mydir 

COPY rails-example-project-master .

RUN apt update && apt install -y nodejs

RUN gem install execjs

RUN bundle install

RUN rails db:migrate

EXPOSE 3000

CMD rails s