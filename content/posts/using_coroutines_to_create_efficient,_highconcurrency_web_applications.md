---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/377_using-coroutines-to-create-efficient-high-concurrency-web-applications.mp4
Speakers: [Matt Spitz]
Tags: [coroutines, gevent, gunicorn, highconcurrency, libevent, pycon, pycon2011,
  wsgi]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011UsingCoroutinesToCreateEfficientHighConcurrency731.png'
Title: 'Using Coroutines to Create Efficient, High-Concurrency Web Applications'
date: '2011-03-11'
---
Using Coroutines to Create Efficient, High-Concurrency Web Applications

Presented by Matt Spitz

Creating high-concurrency python web applications is inherently difficult for
a variety of reasons. In this talk, I'll discuss the various iterations of
application server paradigms we've used at meebo, the advantages/disadvantages
of each approach, and why we've settled on a coroutine-based WSGI setup to
handle our high-concurrency web applications going forward.

Abstract

There are a number of ways in which to create a web application in python.
Some examples include a straight-up CGI scripts that run anew with each
request, preforked Apache workers that each handle multiple requests, and
using an asynchronous web framework like Twisted.

At meebo, we've settled on using gunicorn, a lightweight WSGI server, which
supports gevent, a coroutine-based network library for python. Gevent
monkeypatches python's system modules to make network requests asynchronous
using an event loop based on libevent. This trick allows the developer to use
a simple blocking CGI as a non-blocking web application that can handle many
concurrent requests.

I'll discuss our iteration process through these approaches to building web
applications, why we ended up choosing gunicorn+gevent, the challenges this
new framework presents, and how we've dealt with them.

