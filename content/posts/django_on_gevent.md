---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=nocGRsytBkk"'
ThumbnailUrl: 'http://i.ytimg.com/vi/nocGRsytBkk/hqdefault.jpg'
date: '2012-09-04'
speakers: [Cody Soyland]
tags: [django, gevent]
---
Gevent is an ultra-fast networking library built on top of the greenlet
module. Greenlets are the ideal solution to making Django's synchronous API
calls possible in a cooperative concurrency environment.

I'll begin with an overview of the models of network programming, including
threading, callbacks, and coroutines. I'll explain how greenlets (coroutines)
work in harmony to provide simple blocking network APIs while not blocking
execution of the entire thread. I'll show how easy it is to integrate other
network services into your app.

As an exploration into using realtime features in Django, I'll demonstrate a
simple realtime collaboration app that uses websockets for communication. I
will show how to integrate ZeroMQ to allow the app to scale beyond a single
server. I will also show how to attach to and monitor your web app using
gevent.backdoor.

