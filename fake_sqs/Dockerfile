FROM registry.service.dsd.io/opguk/base:latest

RUN apt-get update && apt-get install -y ruby
RUN gem install fake_sqs --no-ri --no-rdoc

ADD  docker/service/fake_sqs /etc/service/fake_sqs
RUN  chmod a+x /etc/service/fake_sqs/run
