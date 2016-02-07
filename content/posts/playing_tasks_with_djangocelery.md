---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=mAXz2kbh_3U'
Speakers: [Mauro Rocco]
Tags: [celery, distributed, django, infrastructure, queueing, rabbitmq, real-time,
  web]
ThumbnailUrl: 'http://i.ytimg.com/vi/mAXz2kbh_3U/hqdefault.jpg'
Title: 'Playing tasks with Django-Celery'
date: '2011-07-13'
---
Celery is an open source task queueing system based on distributed message
passing.

I will talk about the tools that Celery offers for task distribution and how
to monitor and manage the system using a Django web interface. This talk will
also focus on how we use Celery at Jamendo and our real solutions to some
common issues you may encounter when developing a back-office based on Celery.

The talk will cover the following topics:

  * A brief overview of Celery and the AMPQ protocol AMPQ protocol overview, Celery introduction: Celery, RabbitMQ code examples

  * The impact of Celery on the Jamendo work-flow; examples with real tasks. Here I will talk about the Jamendo back-office infrastructure and some of our common tasks. I will discuss the improvements made by introducing a new back-office system based on Celery. I will show some code snippets and go over some real scenarios.

  * Overview of the Django Celery admin interface and some Jamendo extensions. Let's talk about the Django-Celery interface that allows one to monitor or schedule tasks directly from the Django admin. I will explain which common additional features are necessary and how to add them.

  * Common "gotchas" we encountered while working with Celery and how we solved them.

  * Global task locks

  * Centralized logging: be able to read all the logs of all celery workers on different servers and filter them for real-time debugging

