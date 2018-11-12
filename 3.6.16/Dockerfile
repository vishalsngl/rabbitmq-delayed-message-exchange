FROM rabbitmq:3.6.16
MAINTAINER Vishal Singal <https://github.com/vishalsngl>

RUN apt-get update

RUN apt-get install -y curl unzip

RUN curl -O https://dl.bintray.com/rabbitmq/community-plugins/3.6.x/rabbitmq_delayed_message_exchange/rabbitmq_delayed_message_exchange-20171215-3.6.x.zip

RUN unzip rabbitmq_delayed_message_exchange-20171215-3.6.x.zip -d $RABBITMQ_HOME/plugins

RUN rabbitmq-plugins enable --offline rabbitmq_delayed_message_exchange

RUN apt-get -y remove curl unzip
