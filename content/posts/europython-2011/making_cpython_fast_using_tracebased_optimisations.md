---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=3uTnXITm-kA'
Speakers: [Mark Shannon]
Tags: [cpython, jit, pypy, vm]
ThumbnailUrl: 'http://i.ytimg.com/vi/3uTnXITm-kA/hqdefault.jpg'
Title: 'Making CPython Fast Using Trace-based Optimisations'
date: '2011-07-13'
---
CPython can be made faster by implementing the sort of optimizations used in
the PyPy VM, and in my HotPy VM. All the necessary changes can be made without
modifying the language or the API.

The CPython VM can be modified to support optimizations by adding an effective
garbage collector and by separating the virtual-machine state from the real-
machine state (like Stackless).

Optimizations can be implemented incrementally. Since almost all of the
optimizations are implemented in the interpreter, all hardware platforms can
benefit. JIT compiler(s) can then be added for common platforms (intel, ARM,
etc.).

For more information see
[http://hotpy.blogspot.com/](http://hotpy.blogspot.com/)
