---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: '"http://youtu.be/tGLSKXfx0m0"'
Speakers: [Ben Shaw]
Tags: [talk]
ThumbnailUrl: 'http://i.ytimg.com/vi/tGLSKXfx0m0/hqdefault.jpg'
Title: '"Python is slow, make it faster with C"'
date: '2014-09-13'
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Ben Shaw:
Python is slow, make it faster with C
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Saturday, 13 Sep 2014 - Track 2 
http://kiwi.pycon.org/

**Audience level**

Intermediate

**Description**

Most people have heard that it's possible to integrate Python with C to give performance boosts to computationally heavy code, but because it seems daunting they've never given it a try. It's actually not as hard as you think. This talk covers some of the different methods of speeding up your code with C, and compares the results to those you can get from other methods, like using PyPy.

**Abstract**

Introduction

As developers, we like to work with Python because it's forgiving, quick to develop for and allows our code to be very dynamic. Unfortunately the trade-off for this magic is lower performance than compiled languages. Python can be sped up by offloading heavy algorithms to compiled C, using specially built C modules utilising the C Python API, or by integrating existing C libraries with using the python ctypes module. It is also possible to speed up Python using alternative interpreters, like PyPy, which uses a JIT compiler.

Pure Python Implementation

First we will take a look at a CPU bound algorithm written purely in Python, and see how it performs. The program reads data and prints results. The time it takes to run this will be considered the worst case scenario.

Pure C Implementation

The same program will be re-written in C, including the input and output logic, and we will compare the time it takes to run against the Python implementation. The results of the C implementation will be considered the best case scenario.

Custom Python Module with C Implementation

Python provides an API, C development headers and special C types, to allow the creation of a specially built bridges between Python and C code. In this example, the algorithm will be written in C, and bridged to Python with a custom Python/C module. Input and output takes place within Python, with C only performing the computation. With this method we can achieve near best-case speeds, at the cost of some additional (and sometimes complicated) C coding.

Bridging To C with ctypes

Introduced in Python 2.5, ctypes allows Python to integrate with pre-built C libraries without custom C code. This approach has the advantage over the custom Python/C Module of not needing to write a lot of boilerplate and bridging code in C. As with the Py/C implementation, C is used only to execute the algorithm, and Python takes care of input and output. Again, performance is close to best-case speeds, but the work to integrate with C is much less.

Alternative Python Implementations

PyPy uses a JIT compiler to offer impressive performance gains. The original Python code will be run through PyPy, and although the results might not be as quite as good as using compiled C, they come close, and the effort-to-gain ratio certainly makes it attractive option.

Conclusion

Each performance boosting option has its pros and cons, and when it's so easy to just use PyPy and get good results, why would you still use C? We'll look at some example use cases for each of the methods presented and why you would choose one over the others.

**Slides**

https://speakerdeck.com/nzpug/ben-shaw-python-is-slow-make-it-faster-with-c