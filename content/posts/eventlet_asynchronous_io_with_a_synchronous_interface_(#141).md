---
Category: 'PyCon US 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2010/244_eventlet-asynchronous-i-o-with-a-synchronous-interface-141.m4v
Speakers: [Donovan Preston]
Tags: [asynchronous, eventlet, greenlet, i/o, pycon, pycon2010]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2010EventletAsynchronousIOWithASynchronousInterface667-479.jpg'
Title: 'Eventlet: Asynchronous I/O with a synchronous interface (#141)'
date: '2010-02-19'
---
Eventlet: Asynchronous I/O with a synchronous interface

Presented by Donovan Preston

Network servers which scale to thousands of simultaneous connections have
always been possible in Python thanks to libraries such as asyncore and
twisted. More recently, FriendFeed's new open source project Tornado has
stirred debate in this area. These libraries allow a Python process to scale
to many simultaneous connections using non-blocking I/O (also known as
asynchronous I/O). However these projects require that the programmer learn a
custom API to abstract away the complexities of using a callback-style API.

Eventlet uses greenlet, which provides coroutines as described in "The Art of
Computer Programming", to implement efficient cooperative concurrency while
retaining synchronous semantics. Eventlet also provides an implementation of
the standard library's socket module. Code written to use Python's standard
socket library can be transparently converted to use nonblocking I/O and green
threads with eventlet. This leads to much greater code reuse and programmer
efficiency.

[http://www.eventlet.net/](http://www.eventlet.net/)

