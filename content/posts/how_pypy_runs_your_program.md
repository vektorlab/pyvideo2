---
Category: 'PyCon ZA 2015'
Copyright: ''
Language: 'English'
SourceUrl: '"http://youtu.be/mHTu723RDNI"'
ThumbnailUrl: 'https://i.ytimg.com/vi/mHTu723RDNI/hqdefault.jpg'
date: '2015-10-02'
speakers: [Maciej Fijalkowski]
tags: [Room 215]
---
In this talk we would like to have a short introduction on how Python
programs are compiled and executed, with special attention towards
just-in-time compilation done by PyPy. PyPy is the most advanced Python
interpreter around, and while it should generally just speed up your programs,
there is a wide range of performance that you can get out of PyPy, ranging from
slightly faster than CPython to C speeds, depending on how you write your
programs.

We will split the talk in two parts. In the first part we will explain
how things work, and what can and cannot be optimized, as well as describe
the basic heuristics of the JIT compiler and optimizer. In the next part we will
do a brief survey of existing tools for looking at performance of Python programs,
with a specific focus on PyPy. We'll mostly focus on vmprof with a brief mention of others.

As a result of this talk, an audience member should be better equipped with
the tools to write new software and improve existing software with performance
in mind.
