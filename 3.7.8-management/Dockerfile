FROM rabbitmq:3.7.8-management
LABEL author="Vishal Singal <https://github.com/vishalsngl>"

RUN apt-get update && apt-get install -y \
    curl \
    unzip \
 && rm -rf /var/lib/apt/lists/*

RUN curl -O https://dl.bintray.com/rabbitmq/community-plugins/3.7.x/rabbitmq_delayed_message_exchange/rabbitmq_delayed_message_exchange-20171201-3.7.x.zip 

RUN unzip rabbitmq_delayed_message_exchange-20171201-3.7.x.zip -d $RABBITMQ_HOME/plugins \
 && rm rabbitmq_delayed_message_exchange-20171201-3.7.x.zip

RUN rabbitmq-plugins enable --offline rabbitmq_delayed_message_exchange

RUN apt-get remove -y \ 
    curl \
    unzip
