# this does not work yet

FROM ruby:2.6.0
EXPOSE 3000
ENV RAILS_ENV=production
RUN apt-get update && apt-get -y install git curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN git clone https://github.com/docker-hy/rails-example-project.git
WORKDIR /rails-example-project
RUN gem install bundler
RUN bundle install
RUN rails db:migrate 
RUN rake assets:precompile
CMD rails s -e production
