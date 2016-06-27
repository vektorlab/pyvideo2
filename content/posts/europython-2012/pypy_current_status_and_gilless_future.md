---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=x6OL88pzjHQ'
Speakers: [A Cuni, Armin Rigo, M Fijalkowski]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/x6OL88pzjHQ/hqdefault.jpg'
Title: 'Pypy: current status and gil-less future'
date: '2012-07-04'
---
In the first part of the keynote we will present the current status of PyPy,
with a particular focus on what happened in the last year. We will give a
brief overview of the current speed and the on-going development efforts. The
second part of the keynote is about one particular feature whose development
is in progress in PyPy: Automatic Mutual Exclusion. What it is needs some
explanation: The GIL, or Global Interpreter Lock, is a well-known issue for
Python programmers that want to have a single program using the multiple cores
of today’s machines. This keynote is not about writing a GIL-less Python
interpreter; although hard, this has been done before, notably in Jython. The
real issue is that writing each and every multi-threaded Python programs is
hard too. The threading module offers locks in several variants, conditions,
events, semaphores… But using them correctly without missing one case is
difficult, impossible to seriously test, often impossible to retrofit into
existing programs, and arguably doesn’t scale. (Other solutions like the
multiprocessing module are at best workarounds, suffering some of the same
issues plus their own ones.) Instead, this keynote is about an alternate
solution: a minimal thread-less API that lets programs use multiple cores,
without worrying about races. This may sound impossible, but is in fact
similar to the API simplification of using a garbage collected language over
an explicitly managed one — what is not minimal is “just” the internal
implementation of that API. I will explain how it can actually be done using
Automatic Mutual Exclusion, a technique based on Transactional Memory. I will
give preliminary results on a modified version of the PyPy Python interpreter
that show that it can actually work. I will also explain how the API is used,
e.g. in a modified Twisted reactor that gives multi-core capability to any
existing, non-thread-based Twisted program.
