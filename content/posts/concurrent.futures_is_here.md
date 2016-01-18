---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=2Ng-UIedZMY"'
ThumbnailUrl: 'http://i.ytimg.com/vi/2Ng-UIedZMY/hqdefault.jpg'
date: '2012-07-06'
speakers: [Andrew Dalke]
tags: []
---
The future is here! Or rather, concurrent.futures became part of the Python
standard library with 3.2. This style of asynchronous programming, also known
as promises, has been around for decades but is only recently becoming popular
in a number of languages and libraries. My presentation is meant for a Python
programmer who knows nothing about futures. I’ll structure it around
processing web server logs, and show several ways to Python code can make more
effective use of a multi-core machine. In some cases the multi-threaded
executor is good enough, but in others the right solution is the multi-process
executor. Because of the unified API, it’s a one line change to switch from
one to the other. It isn’t hard to write your own executor for different
compute models. I’ll show that by developing a new one which works on top of
the PiCloud API. At the end I’ll describe some of the more experimental work
I’m doing to use promises in a dependency graph, where certain computed
properties are dependent on others. Even though concurrent.futures came in
3.2, Python 2.x users can use the API through Alex Grönholm’s ‘futures’
backport.

