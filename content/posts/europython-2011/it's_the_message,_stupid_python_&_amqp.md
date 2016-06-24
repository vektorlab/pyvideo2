---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=dIwsKYNbtnI'
Speakers: [Muharem Hrnjadovic]
Tags: [amqp, asynchronous, patterns, performance, queues, scalability, technology]
ThumbnailUrl: 'http://i.ytimg.com/vi/dIwsKYNbtnI/hqdefault.jpg'
Title: 'It''s the message, stupid: python & amqp'
date: '2011-07-13'
---
Messaging is a well established domain in information technology and can
greatly improve the scalability and throughput of a system when employed
appropriately. Message queues can be used to achieve

  * spatial decoupling i.e. the systems that produce and consume messages may be deployed on different machines, networks, continents etc.
  * temporal decoupling i.e. a system can enqueue a message and carry on without waiting for the message consumer.

We use e.g. messaging in [OpenQuake](http://openquake.org) to distribute
calculations of [seismic hazard](http://openquake.org/about/gem/) and the
respective risk to human lives and infrastructure.

There is a huge number of messaging patterns identified in the
[industry](http://www.amazon.com/dp/0321200683/) and a small selection of
these will be presented to whet your appetite :-)

[AMQP](http://www.amqp.org/) is a fairly new and open messaging standard with
a number of freely available open source message brokers
([RabbitMQ](http://www.rabbitmq.com/), [ZeroMQ](http://www.zeromq.org/),
[qpid](http://qpid.apache.org/) etc.) with different features and performance
trade-offs.

In the course of the presentation you will be - introduced to AMQP concepts
and jargon - introduced to available Python AMQP bindings (focussing on an
asynchronous ([txAMQP](https://launchpad.net/txamqp)) and a synchronous
variant (most likely [kombu](http://ask.github.com/kombu/)) - shown code
examples demonstrating how to use these Python bindings

The presentation (45 minutes in total) is structured as follows:

  * 7.5 minutes for messaging concepts and patterns
  * 7.5 minutes for AMQP concepts
  * 5 minutes for an overview of the Python bindings for AMQP
  * 10 minutes for txAMQP examples (asynchronous bindings)
  * 10 minutes for kombu examples (synchronous bindings)
  * 5 minutes for questions

References:

  * [http://www.amqp.org/](http://www.amqp.org/)
  * [http://www.rabbitmq.com/](http://www.rabbitmq.com/)
  * [http://www.zeromq.org/](http://www.zeromq.org/)
  * [http://qpid.apache.org/](http://qpid.apache.org/)
  * [https://launchpad.net/txamqp](https://launchpad.net/txamqp)
  * [http://ask.github.com/kombu/](http://ask.github.com/kombu/)
  * [http://www.amazon.com/dp/0321200683/](http://www.amazon.com/dp/0321200683/)

