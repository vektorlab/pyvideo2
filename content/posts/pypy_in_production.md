---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=nTpte3_jNO0"'
Speakers: [Antonio Cuni, Armin Rigo]
Tags: [cpython, ctypes, cython, extensions, pypy, stackless]
ThumbnailUrl: 'http://i.ytimg.com/vi/nTpte3_jNO0/hqdefault.jpg'
Title: '"PyPy in production"'
date: '2011-07-13'
---
The PyPy project has recently gathered a lot of attention for its progress in
speeding up the Python language - it is the fastest Python interpreter, and
the most compatible and most stable 'alternative´ one. No longer merely a
research project, PyPy is now suitable for production use. We are working on
improvements on calling into C libraries and generally integrating with the
existing Python extensions ecosystem.

We will give an overview on how the tracing Just-in-Time compiler works in
PyPy. From there, we will then focus on what the PyPy project has achieved,
particularly in the past two years:

  * most Python benchmarks run much faster than with CPython or Psyco

  * the real-world PyPy compiler toolchain itself (200 KLocs) runs twice as fast

  * already supports 32 and 64bit x86 and is in the process of supporting ARM

  * full compatibility with CPython (more than Jython/IronPython)

  * full (and JIT-ed) ctypes support to call C libraries from Python

  * supports Stackless Python (in-progress)

  * new "cpyext" layer which integrates existing CPython C extensions

  * an experimental super-fast JIT-compilation of calls to C++ libraries

We want to reserve time for discussing potential future work like SWIG and/or
Cython compatibility and other areas brought up by the audience. There are
many interesting details that can be explored further; we will focus on the
points the audience is most interested in.

For more info:

  * [http://pypy.org/](http://pypy.org/)

  * Our blog: [http://morepypy.blogspot.com/](http://morepypy.blogspot.com/)

  * Eureka program: [http://www.eurostars-eureka.eu/](http://www.eurostars-eureka.eu/)

_Eurostars Eureka is our funding source since 2009. It is a cross-European
funding collaboration that targets small firms which produce research._

