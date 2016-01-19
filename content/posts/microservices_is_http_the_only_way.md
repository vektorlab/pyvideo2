---
Category: 'Kiwi PyCon 2015'
Copyright: 'CC BY-SA'
Language: 'English'
SourceUrl: '"http://youtu.be/O1qaoykYIXY"'
Speakers: [Ben Shaw]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/O1qaoykYIXY/hqdefault.jpg'
Title: '"Micro-Services: Is HTTP the only way?"'
date: '2015-09-05'
---
Introduction
============

Over the past few years, micro-services have been gaining popularity due to their advantages over traditional monolithic architectures. It becomes easier to horizontally scale the heavier portions of an application; you're not tied to the same OS or programming language for the entire application, meaning you can easily slot in the best tool for the job; and finally, you can quickly build the entire application in dynamic yet less performant languages, then rebuild any bottlenecks with faster (but slower to develop) languages.

As a basic example, rather than directly communicating with a database for user authentication, a web front-end would make an HTTP request to another lightweight REST service to check credentials.


An Example Application
======================

In order to elucidate the difference between monolithic and micro-services, we will use a simple Social-Network web application that allows users to post 141 character messages. A user must first sign up, then log in with a username and password, then they can post their messages publicly. A user can then follow any other user, and receive real time updates when that user posts. While the behaviour is simple, there are a number of different concepts that are explored: template rendering, user signup and authentication, data storage and notification delegation.


A Monolithic Version
======================

The first version of the will be a single Django application. The talk does not go into detail on the source code, instead briefly discusses the views, databases (tables and queries) and overall architecture at a high level.


The HTTP Micro-Service Version
===============================

In order to deconstruct the monolith into micro-services, we look at different functions of the application: message viewing, user signup and authentication, data storage and search, and user notification. Django is kept as the front-end, but the databases for authentication, data storage and searching and user-follows are each transformed into their own micro-service. Flask is used as the HTTP framework for these services, with SQLAlchemy for database as necessary. Some source code is discussed (mostly in terms of standard Django database access c.f. HTTP) but this is also quite high level. The talk will also cover what HTTP comes with "out of the box", in terms of authentication, deployment and scalability.


Alternative Transports
======================

After the micro-services have been split, we can start to think about different transports that might be more appropriate (or at least more interesting) in some circumstances.


Introducing a Message Queue
---------------------------

From a user perspective, HTTP is a synchronous protocol, so making other synchronous HTTP calls inside an HTTP handler doesn't introduce much complexity. Message queues, on the other hand, are asynchronous by nature. We look at using message queues for delegating user notifications (which don't require a response, and are easy to handle), then for authentication, data storage and searching – each requiring a slightly different "level" of "synchronicity" and a need to be shoehorned into HTTP differently. We'll look at code for message producing and consuming and discuss architecture again.

Message queues are already widely used for handling intensive background tasks, so we'll look at how they compare to HTTP in this application (for security and deployment), and briefly also talk about cross-platform compatibility.


Lower Down the Stack - Raw Sockets
----------------------------------

If, for some reason, the overhead of HTTP or a message queue is too high, direct socket communication might be better. We'll look at a Python TCP server for user authentication, and a UDP server for handling user notifications, and example code for both. Also discussed are the security implications (it's DIY all the way), performance, and how you might scale these.


Conclusion
==========

Finally we'll look at a comparison overview for all these different methods and summarise with the pros and cons of each.
