---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=a6oHHGIV3r4'
Speakers: [Caroline Tice]
Tags: [api, embedded]
ThumbnailUrl: 'http://i.ytimg.com/vi/a6oHHGIV3r4/hqdefault.jpg'
Title: 'Combining Embedded and Interactive Python in a Debugger:  A Case Study'
date: '2011-07-24'
---
LLDB is an open source compiler currently under development. LLDB incorporates
Python in several different ways: From the command line, one can drop into an
interactive Python script interpreter, entering normal Python interactive
commands and having them interpreted and executed. In addition, the LLDB
debugger has a programming API that allows users to call actual debugger
functions and access real debugger objects. This API is run through SWIG and
converted into a Python module that gets automatically imported into the
interactive interpreter inside LLDB. The upshot of this is that, in the Python
mode, users can call the API functions as if they were regular Python
functions. This is turn means that users can do things like hit a breakpoint,
call the appropriate API functions to get the actual current frame object,
check to see if the caller function several frames up the stack is a
particular function, and if so, perform some other interesting action. LLDB
also allows for breakpoint commands to be written in Python (which therefore
allows them to call the API functions), as well as having a command that
interprets and executes a single line of Python.

Because the API and all of the debugger functionality is available in a Python
module, it is also possible to write a debugger front end completely in Python
and have it import the LLDB module and call the LLDB API functions (which
calls into the LLDB shared library), to create a new debugger front end. Our
test suite takes advantage of this to run tests on the LLDB library without
having to start up an interactive LLDB debubgger session.

There were many interesting problems encountered and overcome in getting all
of this to work. LLDB combines both interactive Python and embedded Python.
There were some interesting things worked out so that a single Python
environment dictionary is used for the entire debugger session: A user can pop
into and out of the interactive interpreter and have access at any time to
anything defined in any previous visit to the interactive interpreter (within
the same debug session); breakpoint commands have access to everything defined
in the interactive session; so do embedded script commands. It gets even more
complicated, because LLDB can have multiple debugger sessions alive at once,
and each debugger session has its own Python interpreter with its own
dictionary and must not be allowed to interfere with another session's state.
In this talk I will discuss how we implemented many of these features in LLDB,
pointing out some of the more interesting problems we encountered and how we
overcame them, and demonstrate it all working in LLDB.

