---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=3329SyR215I'
Speakers: ["Michael K\xF6nig"]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/3329SyR215I/hqdefault.jpg'
Title: 'Embedding Python: Charming the Snake with C++'
date: '2014-07-23'
---
Python with its huge standard library and sophisticated packages developed by its thriving community has become an incredibly useful tool for data scientists. At Blue Yonder, we value Python for the ease with which we can access and combine machine learning algorithms to build accurate prediction models.

To get the most business value out of the use of Python, we strive to rid our model developers from all burdens outside their core expertise, i.e., developing statistical models. To leverage our existing infrastructure, essentially a distributed scheduling system written in C++, we decided to embed a Python interpreter in our application. The goal was to let developers use the language best suited for their problem, and to let them incorporate code created by others even if it is not written in the same language.

In this presentation, I will talk about a few obstacles which we had to overcome in integrating the (C)Python interpreter in our C++ program, e.g., clean resource management, error handling, and broken features in the interpreter's API. I will show how we employed features from the [Boost Python C++ library](http://www.boost.org/doc/libs/1_55_0/libs/python/) not only for simple data exchange, but also for more powerful concepts such as data sources. Finally, I will demonstrate how C++ objects can be used to seamlessly interact with Python, for example to use Python's logging package as usual while the actual logging is handled by our C++ application.

With this combination of both worlds, we achieved a desirable mix of virtues: safe, reliable operations; good run-time performance; fast development; and highly expressive, unit testable core domain logic.