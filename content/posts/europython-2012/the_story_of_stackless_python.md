---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=pDkrkP0yf70'
Speakers: [Armin Rigo, C Tismet]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/pDkrkP0yf70/hqdefault.jpg'
Title: 'The story of stackless Python'
date: '2012-07-05'
---
This talk gives a good overview of the status of Stackless Python: Its history
from the beginning, its current status and its future development to be
expected. A discussion and comparison with similar approaches like Greenlet,
Eventlet and how they relate is also included. Stackless Python 1.0 was
started in 1998 as an implementation of true continuations, with all implied
complications. In 2002, Stackless 2.0 was born, a complete rewrite.
Continuations were abandoned in favor of the much easier to comprehend
tasklets - one-shot continuations that could resume their current state just
once, like Coroutines. In 2004, Stackless 3.0 was created, which merged the
2.0 features with a new concept: so-called “Soft-Switching”, which made the
Pickling of Program State” possible. As a consequence, a few recent
application make solely use of Program State Pickling, which changes the
purpose of Stackless Python quite a bit. One example of this is the “Nagare
Web Framework” which will be shown in examples. In the light of the popularity
of a Stackless spin-off, called “Greenlet”, the concept of a new Stackless
branch will be depicted: Stackless, written as a pure extension module on top
of Greenlets, which includes State Pickling - a feature that seemed to be
impossible to implement without changing CPython. But the impossible and ways
to get around it was always a major topic in this project, which is going to
augment what Stackless on PyPy already can do. Christian Tismer, creator of
Stackless Python Perhaps with Armin Rigo as a guest, talking about Stackless
status in PyPy. Otherwise, I will insert this myself. cheers – Chris

