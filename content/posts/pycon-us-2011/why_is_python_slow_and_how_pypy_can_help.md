---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/427_why-is-python-slow-and-how-pypy-can-help.mp4
Speakers: [Alex Gaynor, Maciej Fijalkowski]
Tags: [jit, pycon, pycon2011, pypy, vm]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011WhyIsPythonSlowAndHowPyPyCanHelp525.png'
Title: 'Why is Python slow and how PyPy can help?'
date: '2011-03-11'
---
Why is Python slow and how PyPy can help?

Presented by Maciej Fijalkowski and Alex Gaynor

PyPy is a virtual machine for Python, featuring an advanced just in time
compiler, which can deliver exceptional performance. This talk is going to be
a deep dive into what exactly makes Python such a hard language to optimize,
how PyPy is organized, and what optimizations our JIT can do (and what it
can't do) for your code.

Abstract

The talk will detail how a python interpreter works internally and why some
operations are costly. We'll go through several python features, how they
work, why they're slow in CPython and how we're fixing it.

The list of mentioned features is not exhaustive, however we will try to focus
at least on the following:

  * Dynamic language - In Python code we have no known types, like a statically typed language. Even operations like "a + b" can do anything, unless we know more about the code, and the types it is operating on.

  * Frame introspection - Frame objects need to be allocated for every function call, and all local variables are stored on the frame, and must be accessible from further down the call stack.

PyPy uses a novel approach called "virtualizables" which makes it possible to
avoid frame allocation in most common cases.

  * Object model - All user defined Python objects have a dictionary which stores their attributes, as does every type. When Python does an attribute lookup this requires at least two dictionary lookups.

In PyPy we use an approach similar to the one used by V8 with hidden classes
(except more PyPy specific) called map dictionaries and other optimizations.

  * FFI calls - Calling C from Python is costly and hard to optimize. In PyPy we expose C APIs to Python code via ctypes. This part explains how we can optimize ctypes calls.

  * array module - Users of CPython's array module probably know it can save them quite a bit of memory, however it's also slower than using a list, due to the overhead of boxing and unboxing on every operations. Here we will tie everything together and describe how the array module is much faster with PyPy's JIT, combining our optimizations to: unbox values, remove the dynamicism within traces, and deliver great performance.
