---
Category: 'PyCon AU 2012'
Copyright: 'http://www.youtube.com/t/terms'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=eOkxLCCbU9w"'
ThumbnailUrl: 'http://i.ytimg.com/vi/eOkxLCCbU9w/hqdefault.jpg'
date: '2012-08-22'
speakers: [Graham Dumpleton]
tags: [bottlenecks, performance]
---
A benchmark of a hello world application is often what developers use to make
the all important decision of what web hosting infrastructure they use. Worse
is that in many cases this is the only sort of performance testing or
monitoring they will ever do. When it comes to their production applications
they are usually flying blind and have no idea of how it is performing and
what they need to do to tune their web application stack.

This talk will provide an overview as to where in your overall request
handling pipeline the main overheads are going to arise. It will then zoom in
and discuss different limiting factors or bottlenecks which can arise within
your WSGI server stack and system that can directly affect the performance of
your Python web application.

Such factors that will be discussed will include:

  * Use of threads vs processes.
  * Number of processors available.
  * Python global interpreter lock (GIL)
  * Amount of memory available.
  * Slow HTTP browsers/clients.
  * Browser keep alive connections.
  * Need to handle static assets.

From this will be provided some general guidelines of what is a good
configuration/architecture to use for different types of Python web
applications.

The importance of continuous production monitoring will also be covered,
ensuring that you know when the performance of your system is dropping off due
to changing traffic patterns as well as code changes you have made in your
actual web application.

