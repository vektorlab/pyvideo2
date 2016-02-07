---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=c08Ee2gQ3pY'
Speakers: [Floris Bruynooghe]
Tags: [bytecode, cpython, vm]
ThumbnailUrl: 'http://i.ytimg.com/vi/c08Ee2gQ3pY/hqdefault.jpg'
Title: 'Exploring CPython''s bytecode'
date: '2011-07-21'
---
The CPython interpreter always compiles your source code to bytecode, usually
stored in .pyc files. This bytecode is then loaded and executed in the CPython
virtual machine.

This talk will explore the bytecode from the outside in. Starting with how to
read a .pyc file, following the steps the interpreter takes to arrive and a
usable python module. It then dives into the structure of the bytecode itself
and the principles of the virtual machine, detailing how the VM executes this
bytecode to do useful work.

Having seen all these details you should have a good idea of the various
innards of CPython and how to manipulate these to create weird, wonderful,
dangerous and occasional useful hacks.

