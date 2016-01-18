---
Category: 'PyCon US 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2010/352_actors-what-why-and-how-161.m4v
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2010ActorsWhatWhyAndHow161560.png'
date: '2010-02-19'
speakers: [Donovan Preston]
tags: [concurrency, eventlet, infrastructure, pycon, pycon2010, rest, scaling, wsgi]
---
Actors: What, Why and How

  
Presented by Donovan Preston

  
Since the dawn of concurrency research, there have been two camps: shared
everything, and shared nothing. Most modern applications use threads for
concurrency, a shared everything architecture.

  
Actors, however, use a shared nothing architecture where lightweight processes
communicate with each other using message passing. Actors can change their
state, create a new Actor, send a message to any Actor it has the Address of,
and wait for a specific kind of message to arrive in it's mailbox.

  
We will discuss the benefits of using the Actor architecture and strategies
for implementing an Actor system in Python.

  
[http://bitbucket.org/fzzzy/python-actors/](http://bitbucket.org/fzzzy/python-
actors/)

