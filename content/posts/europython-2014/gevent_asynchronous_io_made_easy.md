---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=0wpYQr-_kqg'
Speakers: [Daniel Pope]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/0wpYQr-_kqg/hqdefault.jpg'
Title: 'gevent: asynchronous I/O made easy'
date: '2014-07-23'
---
It has been claimed "Callbacks are the new GOTO". Most asynchronous IO libraries use callbacks extensively.

gevent (http://www.gevent.org) uses coroutines to provide highly scalable asynchronous I/O with a synchronous programming model that doesn't need code changes and callbacks. By elegantly monkey patching the Python standard library, both your code and all pure Python libraries become asynchronous too, making a separate collection of protocol implementations (in the style of Twisted) unnecessary.

Code written like this is easier to understand, particularly for more junior developers. Crucially, IO errors can be raised at the right places.

I will be introducing gevent's programming model, why it's easier, walk through simple code samples, and discuss experiences and metaphors for programming with it.
