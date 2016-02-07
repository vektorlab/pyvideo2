---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=aNl7GrnKTcs'
Speakers: ["P\xE9ter Szab\xF3"]
Tags: [concurrence, cpython, design, greenlet, stackless, testing]
ThumbnailUrl: 'http://i.ytimg.com/vi/aNl7GrnKTcs/hqdefault.jpg'
Title: 'Emulating Stackless and greenlet with each other'
date: '2011-07-21'
---
Stackless Python and the greenlet package for CPython are two different
implementations of coroutine support for Python. (Coroutines are fundamental
building blocks of I/O frameworks like gevent, Eventlet, Concurrence and
Syncless to conveniently handle thousands of socket connections at a time
without creating threads.) Stackless and greenlet implement a different
interface. However, each is powerful enough so that it can be used to emulate
the other one. In this talk we explore the differences and discuss design
decisions and testing strategies of the emulations we have implemented.

[Slides](http://syncless.googlecode.com/svn/trunk/doc/slides_2011-06-20/pts_em
u_coro_2011-06-20.html)

[Slides for the bonus sub-talk](http://syncless.googlecode.com/svn/trunk/doc/s
lides_2010-11-29/pts_coro_2010-11-29.html)

