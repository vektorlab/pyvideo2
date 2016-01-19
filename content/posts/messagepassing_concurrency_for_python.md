---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=EsSdtvIGWAA"'
Speakers: [Sarah Mount]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/EsSdtvIGWAA/hqdefault.jpg'
Title: '"Message-passing concurrency for Python"'
date: '2014-07-22'
---
Concurrency and parallelism in Python are always hot topics. Early Python versions had a threading library to perform concurrency over operating system threads, Python version 2.6 introduced the multiprocessing library and Python 3.2 has introduced a futures library for asynchronous tasks. In addition to the modules in the standard library a number of packages such as gevent exist on PyPI to implement concurrency with "green threads". 

This talk will look the variety of forms of concurrency and parallelism. When are the different libraries useful and how does their performance compare? Why do programmers want to "remove the GIL" and why is it so hard to do? In particular this talk will give an overview of various forms of message-passing concurrency which have become popular in languages like Scala and Go. A Python library called python-csp which implements similar ideas in a Pythonic way will be introduced and we will look at how this style of programming can be used to avoid deadlocks, race hazards and "callback hell".