---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/388_jython-concurrency.mp4
Speakers: [Jim Baker]
Tags: [concurrency, java, jython, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011JythonConcurrency940.png'
Title: '"Jython Concurrency"'
date: '2011-03-11'
---
Jython Concurrency

Presented by Jim Baker

Jython is arguably the best Python implementation to target concurrent code.
Jython has no GIL, it leverages the Java platform to provide robust support
for concurrency in its runtime, and it enables access to a set of high-level
abstractions from Java. This talk will walk through at the extreme level
pertinent Jython implementation details and a series of examples, including
Java integration.

Abstract

Jython implements the Python language, but we leverage the underlying Java
platform to provide an opionated alternative to CPython in our support of
concurrency.

Because of the GIL and related infrastructure, CPython cannot use a model in
which threads perform concurrent computation defined in Python on shared
objects in the same process. (Of course, there are workarounds, such as
multiprocessing or using C extensions.)

In contrast, there's no GIL in Jython. Jython instead embraces threads,
provides extensive support for managing their execution and coordination
through standard Java platform functionality (java.util.concurrent), and
threaded code works well with Jython's implementation of standard mutable
collection types. Lastly, the underlying JVM provides extensive
instrumentation as well as the ability to set a variety of parameters,
including choice of GC. There are also the inevitable pitfalls that might be
seen in complex architectures, such as around the use of ClassLoaders.

This talk will go into a detailed discussion of some of the interesting
ramifications of these design points and how they can be effectively applied
to write concurrent code, as illustrated through a variety of short examples.

