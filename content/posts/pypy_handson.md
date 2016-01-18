---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=qcqEAE4QoeA"'
ThumbnailUrl: 'http://i.ytimg.com/vi/qcqEAE4QoeA/hqdefault.jpg'
date: '2011-07-21'
speakers: [Antonio Cuni, Armin Rigo]
tags: [cd, cpython, extensions, hg, jit, optimize, pypy, setup.py, tutorial]
---
The session is divided into two parts, of roughly 2 hours each. People who are
interested only in the first part, can leave the session after it. However,
the first part is a prerequisite for the second one, thus people are not
advised to join in the middle of the session.

The session is meant to be highly interactive. People are invited to bring
their own laptop and try things by themselves.

## Part 1: Run your application under PyPy

This tutorial is targeted to Python users who want to run their favorite
Python application under PyPy, and exploit the most of it. The following
topics will be covered:

    
    - how to fix/avoid CPython implementation details (e.g., refcounting)
    
    - general overview of how the PyPy JIT works
    
    - how to optimize your program for the PyPy JIT
    
    - how to view and interpret the traces produced by the JIT
    
    - how to tweak the parameters of the JIT and the GC
    
    - how to use existing CPython C extensions on PyPy, and fix them if necessary
    

## Part 2: Write your own interpreter with PyPy

PyPy is not only a Python interpreter, but also a toolchain to implement
dynamic languages. This tutorial is targeted to people who want to implement
their own programming languages, or who simply want to know more about how the
PyPy JIT works internally.

The students will be given the source code for a toy language implemented in
RPython. They will learn:

    
    - how to translate it to C using the PyPy translation toolchain
    
    - what are the "hints" needed by the JIT generator, and how to place them
    

Then, they will be challenged to add the proper hints to the toy interpreter,
to get the best result with the JIT.

**THINGS TO DO BEFORE THE TRAINING**

You are encouraged to bring your laptop to the training session.

Make sure that the following prerequisites are met:

  * Install PyPy 1.5:

    * [http://pypy.org/download.html](http://pypy.org/download.html)

    * [http://doc.pypy.org/en/latest/getting-started.html#installing-pypy](http://doc.pypy.org/en/latest/getting-started.html#installing-pypy)

  * Make sure that `setuptools` or `distribute` are installed (look at the URL above for instructions)

  * Clone the pypy repository, and update to the 1.5 version::

$ hg clone [http://bitbucket.org/pypy/pypy](http://bitbucket.org/pypy/pypy)

$ cd pypy

$ hg up -r release-1.5

  * Clone the jitviewer repository and install it on pypy::

$ hg clone
[http://bitbucket.org/pypy/jitviewer](http://bitbucket.org/pypy/jitviewer)

$ cd jitviewer

$ /path/to/pypy-1.5/bin/pypy setup.py develop

If you intend to follow also the second part ("Write your own interpreter with
PyPy"), you need to make sure you have a working [developing
environment](http://doc.pypy.org/en/latest/getting-started-python.html
#translating-the-pypy-python-interpreter)

