---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=4Ztq-Yz1ero'
Speakers: [O Vilaplana]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/4Ztq-Yz1ero/hqdefault.jpg'
Title: 'Tornado in Depth'
date: '2012-07-04'
---
Tornado is a non-blocking light-weight web server and framework. There’s been
many introductory talks about it, and it’s time to look deeper into it: not
just what Tornado does, but how it does it and what can we learn from it when
designing our own concurrent systems. We’ll cover each topic in two parts:
first we’ll see how to use a certain feature in our applications; then, we’ll
dig into Tornado’s source code to see how it really works. How much time we’ll
spend in the “how to use” will depend on the audience’s knowledge of Tornado.
Getting Started: quickly get a simple Tornado application up and running.
We’ll keep digging into, changing and poking this Application for most of the
talk. An Application Listens: what an Application is, how does Tornado start
it and how does it process its requests. Application and IOLoop: we’ll look at
how the IOLoop receives the connections from the users and passes them on to
the Applications. Scheduled Tasks: we’ll see how to schedule tasks and how the
IOLoop will run them. Generators: we’ll learn to use generators to handle the
responses of our asynchronous calls, and how they work with the IOLoop.
Websockets: how to use them and how they work. IOStream: how do Tornado’s non-
blocking sockets work. Database: how to use non-blocking sockets to connect to
a MySQL or MongoDB database.

