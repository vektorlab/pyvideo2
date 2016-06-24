---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=BBAfIYpDMX4'
Speakers: [Nick Barkas]
Tags: [requests, scalability]
ThumbnailUrl: 'http://i.ytimg.com/vi/BBAfIYpDMX4/hqdefault.jpg'
Title: 'Spotify: Horizontal scalability for great success'
date: '2011-07-13'
---
If you run on CPython, it's not possible to get a single-process,
multithreaded Python program to use more than one CPU core at a time because
of the Global Interpreter Lock (GIL). A common way of dealing with this is to
run one instance of a Python program for each core a machine has and spread
the load amongst those processes. This forces developers to write simple,
stateless programs that naturally scale out to many many servers when needed,
while also not having to think about things like locking and thread
scheduling.

I'll discuss some tools and methods Spotify's backend uses for managing
multiple identical server processes as well as load balancing with DNS, proxy
servers, and using hashing to send repeated requests to the same process. I
will also talk about the difficulties that arise when you really need to share
data or state between processes, and how they can be dealt with.

