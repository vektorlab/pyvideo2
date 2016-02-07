---
Category: 'PyCon ZA 2015'
Copyright: ''
Language: 'English'
SourceUrl: 'http://youtu.be/b8Cj5-LieH0'
Speakers: [Carl Scheffler]
Tags: [Room 215]
ThumbnailUrl: 'https://i.ytimg.com/vi/b8Cj5-LieH0/hqdefault.jpg'
Title: 'Distributed pub-sub infrastructure with Apache Kafka'
date: '2015-10-01'
---
[Apache Kafka](http://kafka.apache.org/) is great for building a large scale distributed data bus. Even a small cluster will happily accept and store thousands of messages per second, and make them available to consumers with low latency.

Kafka was chosen as the solution to our publish-subscribe infrastructure at [Takealot.com](http://www.takealot.com/). It supports our event-driven systems on the website, in the warehouses and in the office, as well as our analytics and machine learning projects.

This talk will

 * introduce the basic Kafka principles that make things work,
 * outline how Kafka fits in with the rest of our architecture,
 * cover some of the practicalities of building Python-based Kafka services,
 * compare the two main Python libraries for Kafka, namely [kafka-python](https://github.com/mumrah/kafka-python) and [pykafka](https://github.com/Parsely/pykafka),
 * demonstrate some practical applications at Takealot.com.

Join in if you are interested in scalable distributed infrastructure.