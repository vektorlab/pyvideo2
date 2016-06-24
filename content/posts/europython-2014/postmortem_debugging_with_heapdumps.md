---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=0Xt-au2QnRg'
Speakers: [Anselm Kruis]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/0Xt-au2QnRg/hqdefault.jpg'
Title: 'Post-Mortem Debugging with Heap-Dumps'
date: '2014-07-25'
---
Post-Mortem Debugging with Heap-Dumps
=====================================

UNIX core-dumps, Windows minidumps and analogous solutions of other operating systems are well established technologies for 
post-mortem defect analysis of native-code processes. In principle those dumps can be used to analyse „interpreted“ 
programs running within a native-code interpreter-process. However in practise this approach is tedious and not always successful \[1\].
Therefore operating system independent dump methods were developed for some „interpreted“ languages \[2\]. 
A prominent example are Java heap dumps \[3\]. 

Unfortunately up to now there was no practically usable dump-method for Python. Various attempts were made 
to utilise OS-level dump methods \[4, 5\]. In 2012 Eli Finer published the Python module *pydump* \[6\].
This module pickles the traceback of an exception and subsequently uses the pdb debugger to analyse the unpickled traceback.
Unfortunately *pydump* fails on PicklingErrors.

In my talk I'll present the Python package [*pyheapdump*](https://pypi.python.org/pypi/pyheapdump). It has the same operation principle as Eli's *pydump*, but 
is an independent implementation. *pyheapdump* uses an extended pickler 
([sPickle](https://pypi.python.org/pypi/sPickle)) to serialise all relevant objects 
of a Python process to a file. Later on a fault tolerant unpickler recreates the objects and a common Python
debugger can be used to analyse the dump. The pickler extensions make it possible to:

 * pickle and unpickle many commonly not pickleable objects [7].
 * replace the remaining not pickleable objects by surrogate objects so that the resulting object graph is
   almost isomorphic to the original object graph.
   
Which objects are relevant? In its default operation mode *pyheapdump* 
uses the frame-stacks of all threads as start point for pickling. Following the 
usual rules for pickling the dump includes all local variables and all objects 
reachable from a local variable and so on. That is usually enough for a successful defect analysis.

Compared with other Python post-mortem debugging methods *pyheapdump* has several advantages:

 * It is a pure Python solution and independent from the operation system.
 * Creation of the pyheapdump and fault analysis can be performed different computers.
 * It is not obstructive. It does not modify / monkey-patch or disturb the dumped 
   process in any way, with the exception of loading additional modules.
 * If used with the Pydev-debugger, it supports multi-threaded applications.
 * If used with the Pydev-debugger and Stackless Python, it supports tasklets. 

The implementation of *pyheapdump* is fairly small, because it draws most of its functionality 
from the underlying sPickle package and from the new Stackless-Support \[8\] of the
Pydev-Debugger. Therefore it is - despite of its short history - already a useful piece of software.

Outline of the talk
-------------------

1.	Introduction to the problem
2.	Previous works
3.	The concept of *pyheapdump*
4.	Live demonstration
5.	Open problems and further development
6.	Questions and Answers

References
----------

1. Andraz Tori, Python, 2011-01-16: *gdb and a very large core dump*, blog at <http://www.zemanta.com/blog/python-gdb-large-core-dump/>
2. David Pacheco, ACM Queue - Programming Languages Volume 9 Issue 10, October 2011: 
   *Postmortem Debugging in Dynamic Environments*, 
   PDF <http://dl.acm.org/ft_gateway.cfm?id=2039361&ftid=1050739&dwn=1&CFID=290171300&CFTOKEN=95099236>
3. Chris Bailey, Andrew Johnson, Kevin Grigorenko, IBM developerWorks, 2011-03-15: 
   *Debugging from dumps - Diagnose more than memory leaks with Memory Analyzer*, 
   PDF <http://www.ibm.com/developerworks/library/j-memoryanalyzer/j-memoryanalyzer-pdf.pdf>
4. Brian Curtin, 2011-09-29: *minidumper - Python crash dumps on Windows*, 
   blog at <http://blog.briancurtin.com/posts/20110929minidumper-python-crash-dumps-on-windows.html>
5. David Malcolm, Fedora Feature, 2010-04-06: *Easier Python Debugging* 
   at <http://fedoraproject.org/wiki/Features/EasierPythonDebugging>
6. Eli Finer, Github-Project, 2012: *pydump* at <https://github.com/gooli/pydump>
7. Anselm Kruis, EuroPython 2011: *Advanced Pickling with Stackless Python and sPickle*,
   archived talk at <https://ep2013.europython.eu/conference/talks/advanced-pickling-with-stackless-python-and-spickle>
8. Fabio Zadrozny, 2013-12-12: *PyDev 3.1.0 released*, 
   blog at <http://pydev.blogspot.de/2013/12/pydev-310-released.html>

