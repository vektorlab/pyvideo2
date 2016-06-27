---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=ZRCjfSIVMNA'
Speakers: [Giles Thomas]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/ZRCjfSIVMNA/hqdefault.jpg'
Title: 'An HTTP request''s journey through a platform-as-a-service'
date: '2014-07-23'
---
PythonAnywhere hosts tens of thousands of Python web applications, with traffic ranging from a couple of hits a week to dozens of hits a second.  Hosting this many sites reliably at a reasonable cost requires a well-designed infrastructure, but it uses the same standard components as many other Python-based websites.  We've built our stack on GNU/Linux, nginx, uWSGI, Redis, and Lua -- all managed with Python.  In this talk we'll give a high-level overview of how it all works, by tracing how a request goes from the browser to the Python application and its response goes back again.  As well as showing how a fairly large deployment works, we'll give tips on scaling and share a few insights that may help people running smaller sites discover how they can speed things up.
