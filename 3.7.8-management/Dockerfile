FROM rabbitmq:3.7.8-management
MAINTAINER Vishal Singal <https://github.com/vishalsngl>

RUN apt-get update

RUN apt-get install -y curl unzip

RUN curl -O https://dl.bintray.com/rabbitmq/community-plugins/3.7.x/rabbitmq_delayed_message_exchange/rabbitmq_delayed_message_exchange-20171201-3.7.x.zip 

RUN unzip rabbitmq_delayed_message_exchange-20171201-3.7.x.zip -d $RABBITMQ_HOME/plugins

RUN rabbitmq-plugins enable --offline rabbitmq_delayed_message_exchange

RUN apt-get -y remove curl unzip
