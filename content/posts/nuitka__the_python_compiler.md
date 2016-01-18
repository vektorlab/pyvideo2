---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=ZDHkla5rllg"'
ThumbnailUrl: 'http://i.ytimg.com/vi/ZDHkla5rllg/hqdefault.jpg'
date: '2012-07-05'
speakers: [K Haye]
tags: []
---
With Nuitka, for the first time, there is a consequently executed approach to
statically translate the full language extent of Python, with all its special
cases, without introducing a new or reduced version of Python. It is compiled,
but with practically 100% compatibility. Function dictionaries work, code
objects exist, frame stack works, exception tracebacks, eval, exec, closures,
nested functions, meta classes, etc. it’s all there, and behaves identical.
First, I would like to start out and explain how I came to write a Python
compiler, why I want it to be 100% compatible, and why I find deviations from
Python unacceptable and out of scope. Then I would like to describe where
difficulties were in the implementation, what Python constructs surprised me,
and where the mapping from Python to C++ left things to desire. In this
project, I learned a lot about Python, it wasn’t easy to get the full CPython
test suite to run. In doing that, I have learned anecdotes and fine details of
Python, that are normally hidden in daily programming, but are still useful to
know. Esp. the work on re-formulating “with” statements, “assert”,
“while"/"for” as generic loops, etc. gives an interesting view on Python
itself. And I would like to present it, also for the insight it gives on
Python. I will give an overview over newly developed infrastructure, aiming
for type inference at compile time, and show existing stuff. I will try and
explain, why I hope to have picked the right approach in this domain. An
interesting side game, is the approach to use XML representations of the
internal node tree of Nuitka to discover regressions/changes in the optimizer.
Then I will also present a project road map, with the milestones for Nuitka,
and why I believe this is the right plan, and how Nuitka is different from
projects like “Cython” and “PyPy”. To round it up, I would like to make a
demonstration of Nuitka, and give an example for how easy it should be to
contribute. As this will be the first time, Nuitka is introduced the PyCON EU
(it was only shown on PyCON DE 2011 so far). And to celebrate that, the
current GPLv3 license will be lifted, and replaced with Apache 2.0 license
(ASF), which is entirely liberal.

