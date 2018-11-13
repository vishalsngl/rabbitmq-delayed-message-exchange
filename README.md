RabbitMQ based on Official image with the corresponding version of Delayed Message Exchange plugin.

## Description
These are RabbitMQ dockerfiles, based on the [Official](https://hub.docker.com/_/rabbitmq) RabbitMQ images. The corresponding version of the Delayed Message Exchange as available on [Community Plugins](https://www.rabbitmq.com/community-plugins.html) has been added and enabled.

## Versions
- [latest](https://github.com/vishalsngl/rabbitmq-delayed-message-exchange/blob/master/latest)
- [3.7.8-management](https://github.com/vishalsngl/rabbitmq-delayed-message-exchange/blob/master/3.7.8-management/Dockerfile)
- [3.7.8](https://github.com/vishalsngl/rabbitmq-delayed-message-exchange/blob/master/3.7.8/Dockerfile)
- [3.6.16-management](https://github.com/vishalsngl/rabbitmq-delayed-message-exchange/blob/master/3.6.16-management/Dockerfile)
- [3.6.16](https://github.com/vishalsngl/rabbitmq-delayed-message-exchange/blob/master/3.6.16/Dockerfile)

## Usage
Since these are based on Official Images, the environment variables can be used as in [Official Images](https://hub.docker.com/_/rabbitmq).
The default RabbitMQ ports are exposed as in the [Official Images](https://hub.docker.com/_/rabbitmq). Sample docker run command is as follows \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`docker run vishalsngl/rabbitmq-delayed-message-exchange:latest`
