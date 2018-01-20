This repository demonstrates, how to receive `STOMP` messages from RabbitMQ via JavaScript, using the RabbitMQ Web STOMP Plugin (https://www.rabbitmq.com/web-stomp.html).

The folder `rabbitmq` contains a Dockerfile, which can be used to build a RabbitMQ Docker image. To make all needed ports accessible, the image can be run like: `docker run -p 15672:15672 -p 15674:15674 <name of docker image>`.

The JavaScript within `index.html` connects via the default settings of RabbitMQ to the broker and subscribes to the queue `messageQueue`. All messages published by this queue are send to the browser and printed.
