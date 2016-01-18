---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=YM4F6sSAu9k"'
ThumbnailUrl: 'http://i.ytimg.com/vi/YM4F6sSAu9k/hqdefault.jpg'
date: '2012-09-04'
speakers: [Amjith Ramanujam]
tags: [debugging, django]
---
This talk will go over some of the ways in which a monitoring system such as
New Relic can be used to focus in on where problems are arising in a Python
web application using a framework such as Django. It will also describe how
you can then use that information to drill down even further by applying
separate debugging tools and techniques rather than monitoring systems.
Debugging tools aren't generally associated with production systems however
and even mentioning them in relation to production systems often makes DevOps
people rather nervous.

The main purpose of the talk therefore is to look at a range of debugging
tools and techniques which can be applied to web applications but also
separate them into what might and might not be realistically used on live
production web applications. It will then describe the use of an embedded
interactive console port as a gateway into a live web application, how one may
setup a set of predefined commands that could be issued against a live web
application, or for the brave, how it could be used to fire up an embedded
Python interpreter prompt or pdb session.

Topics to be touched on would include:

  * Browser viewable error pages.
  * Browser based debuggers.
  * Python interactive debuggers.
  * Post-mortem exception analysis.
  * Methods for dumping Python stack traces
  * Methods for dumping C stack traces.
  * Methods for analyzing thread utilization.
  * Interactive process introspection tools.
  * Error reporting and logging services.
  * Performance monitoring services.

