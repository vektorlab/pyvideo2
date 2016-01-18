---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=xbWBIudWRxQ"'
ThumbnailUrl: 'http://i.ytimg.com/vi/xbWBIudWRxQ/hqdefault.jpg'
date: '2012-09-06'
speakers: [Joshua Ginsberg]
tags: [django, redis]
---
Getting your Django app to a v1.0 release means focusing on function and user
experience before prematurely focusing on optimization. But once it's off the
ground, the Redis key-object store provides a versatile and functional way to
take your app to the next level of performance and function with minimal
engineering.

[Redis](http://redis.io) is an in-memory key-object database that can perform
standard operations on simple values, lists, sets, hash maps, and scored sets
with incredible efficiency. While it cannot and should not replace SQL for
schema-defined, persistent data storage, it can provide dramatically faster
operational efficiency for volatile, temporary, or rapidly changing data with
minimal coding required.

This talk begins by introducing Redis, its basic featureset, and the data
types and operations it supports. We'll cover some high-level guidelines and
strategies for identifying where Redis may be an appropriate performance-
enhancing solution. We then cover the out-of-the-box ways that Redis can
improve a Django application as a cache, session store, Celery broker, and
more. We'll then proceed to more advanced usage possibilities, implementing a
real-time websocket based messaging solution, scripting within Redis using its
embedded Lua interpreter, and connecting Redis to PostgreSQL using Foreign
Data Wrappers to efficiently blend SQL tables with Redis data.

By the end of the presentation, you should be able to use all of the data-
structures offered by Redis, to identify opportunities within you codebase
that Redis may offer simple but dramatic efficiency improvements, and to
envision how advanced Redis usage may bring new and cutting-edge functionality
to your project.

Redis was developed by [Salvatore Sanfilippo](http://twitter.com/antirez) and
[Pieter Noordhuis](http://twitter.com/pnoordhuis), who are both supported by
VMWare to develop the database full-time. Redis has excellent [Python
bindings](https://github.com/andymccurdy/redis-py/) developed by Andy McCurdy.

