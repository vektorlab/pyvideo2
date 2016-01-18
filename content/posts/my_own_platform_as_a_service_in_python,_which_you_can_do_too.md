---
Category: 'Kiwi PyCon 2015'
Copyright: 'CC BY-SA'
Language: 'English'
SourceUrl: '"http://youtu.be/AxTeVemFBkQ"'
ThumbnailUrl: 'https://i.ytimg.com/vi/AxTeVemFBkQ/hqdefault.jpg'
date: '2015-09-05'
speakers: [Lee Begg]
tags: []
---
Over the last couple of years I have evolved my own Platform as a Service (PaaS) for hosting Django apps, and you can run it too.

I use Nginx, Circus, Chaussette, and Django, with some support from Django-environ and deployment automation using Fabric. All of that except Nginx are written in Python. Systemd is a new init process coming.

* Circus is a process and socket manager, and gives a nice way to scale processes. 
* Chaussette WSGI server works well with Circus, as Circus can pass the socket to it.
* Django-environ it's a library that parses environment variables or files with key-value pairs. Environment variables are used on some PaaS, but the file support I find very useful.
* Fabric is a framework for writing system commands to be run on remote hosts, and is great for automating system administration.
* Systemd is a new "init" process for Linux and offers some interesting possibilities for hosting Python webapps.