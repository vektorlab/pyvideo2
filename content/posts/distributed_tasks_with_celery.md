---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/452_distributed-tasks-with-celery.mp4
Speakers: [Ryan Petrello]
Tags: [amqp, celery, pycon, pycon2011, queueing]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011DistributedTasksWithCelery711.png'
Title: 'Distributed Tasks with Celery'
date: '2011-03-11'
---
Distributed Tasks with Celery

Presented by Ryan Petrello

Celery is an open source task queueing system based on distributed message
passing, especially using the AMQP protocol. This talk will focus on the need
for task distribution, the tools celery provides to meet those needs, and an
in-depth discussion of how we've used celery at ShootQ to improve the
efficiency and reliability of our background processes.

Abstract

The talk (including time for questions) will last approximately 30 minutes and
will focus on the following topics:

  * The need for distributed tasks in real world systems, especially in a web application environment. This portion of the talk will describe examples where the traditional request-response model of the web can be improved with background processing. 
  * A brief overview of traditional distributed message passing models and the AMPQ protocol. 
  * An overview of Celery and the variety of tools it provides for task distribution, scheduling, and execution. This portion of the talk will also review production-oriented components of Celery, such as monitoring, error detection/reporting, and error recovery. 
  * Real world discussion of several problems we solved at ShootQ using Celery including before-and-after looks at our implementations. 
  * Common pitfalls and gotchas we encountered while working with Celery. 

