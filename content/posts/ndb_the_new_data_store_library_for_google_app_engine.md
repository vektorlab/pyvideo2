---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=HiOp8KQLcgM'
Speakers: [Guido van Rossum]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/HiOp8KQLcgM/hqdefault.jpg'
Title: 'NDB: the new data store library for Google App Engine'
date: '2012-07-06'
---
NDB is a new Python client library for the Google App Engine Datastore. NDB
has an integrated multi-level cache, supports synchronous and asynchronous
calls, automatically batches requests, and several ways of storing structured
data. The thrust for developing NDB was the realization that the original
Python datastore client library, “db”, had some architectural and design flaws
which were hard to fix due to strict backward compatibility requirements. But
in the process, NDB became much more than an improved db library. NDB offers a
new paradigm for asynchronous APIs, based on coroutines implemented using
Python’s “yield” expression (and a simple event loop). It also supports a
flexible way to create new Property classes by subclassing existing Property
classes.

