---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=6jD34p8PokU"'
Speakers: [Giovanni Bajo]
Tags: [cpython, debugging, design, memory, performance, profiling, 'python,']
ThumbnailUrl: 'http://i.ytimg.com/vi/6jD34p8PokU/hqdefault.jpg'
Title: '"Debugging and profiling techniques"'
date: '2011-07-20'
---
This talk will give on overview over some common problems related to profiling
and debugging CPython applications (especially desktop-based ones).

The following subjects will be covered:

  * Debugging of memory/resource leaks (circular references, **del**, weakref, garbage collector, etc.). We will show in details how the memory management of Python objects work and we will show a few tricks to track memory leaks
  * Python code profiling (profile/hotshots/cProfile, design of small tests, etc.). We will show how to measure, profile, and analyse an application to spot performance problems and solve them.
  * Post-mortem step-by-step debugging of C/C++ extension under Windows. We will show how to setup Visual Studio for debugging, how to see a traceback in case of an unexpected segfault, and how to further debug and solve the crash.

This talk is aimed at intermediate Python programmers, who have already
developed non-trivial Python applications but have never "jumped through" the
interpreter abstraction layer. If you feel a little lost when you see a
segfault from a Python program or you don't have a clear idea how memory is
collected in Python, this talk is perfect for you.

