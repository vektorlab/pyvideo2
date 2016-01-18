---
Category: 'DjangoCon 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/djangocon-2010/39_massaging-the-pony-message-queues-and-you.flv
ThumbnailUrl: 'http://a.images.blip.tv/Robertlofthouse-MassagingThePonyMessageQueuesAndYou879.png'
speakers: [Shawn Rider]
tags: [celery, djangocon, djangocon2010, messagequeues, queues, rabbitmq]
---
Massaging the Pony: Message Queues and You

Presented by Shawn Rider

Message queues are a potential solution for any site that needs to facilitate
robust asynchronous operations on your website including carrying out
intensive or long-running actions or synchronizing off-site services. We will
look at how PBS has used Celery and RabbitMQ to provide more reliable service
and how to set up a robust message queue solution in a cloud hosting
environment.

Abstract

In maintaining several different site projects written in Django over the past
four years, the PBS Education team repeatedly found the need for the ability
to create asynchronous processes that could handle long-running actions and
mission-critical synchronization. We needed a way to handle tasks such as
generating reports on large data sets and executing remote processes on fussy
third-party services. The clear solution to the problems we encountered was to
implement a robust message queue solution.

Message queues allow sites to execute processes outside the normal HTTP
request cycle and then deliver the results of those processes in a variety of
ways. After a survey of all available message queue solutions we settled on a
combination of Celery and RabbitMQ to create a reliable, always-available
system that can handle mission-critical tasks. We can easily develop against a
message queue in our development builds, and we have an infrastucture based in
a cloud hosting service that allows us to rely on the message queue without
reservation.

In this talk will will look at what a message queue does for your site, how to
implement a message queue in your Django code, and how to set up a reliable
message queue infrastructure on your servers. We will show examples from some
of our sites at PBS so it is clear how message queues work and to present some
common use cases that warrant a message queue solution. We will also discuss
some of the design patterns that made it easy to switch to message queue based
processing for discreet tasks, as well as some of the things we learned that
have made the solution even easier to implement for new tasks.

