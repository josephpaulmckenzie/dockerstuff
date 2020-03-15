FROM lambci/lambda:build-ruby2.5

RUN yum install -y postgresql postgresql-devel mysql mysql-devel
RUN gem update bundler
RUN gem install bundler
ADD Gemfile /var/task/Gemfile
RUN bundle install --path /var/task/vendor/bundle --clean

