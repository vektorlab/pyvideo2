---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=kT34QMil-FQ'
Speakers: [Thomas Aglassinger]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/kT34QMil-FQ/hqdefault.jpg'
Title: 'Solution oriented error handling'
date: '2014-07-22'
---
Traditionally error handling is regarded an annoyance by developers because it removes the focus from the already difficult enough productive parts of the code to parts that ideally will never be called. And even if, end users seem to be ignore the error messages and just click "Ok" or call the help desk.

Solution oriented error handling uses Python's existing try/catch/finally idiom, with statement, assert statement and exception hierarchy in a way that keeps the code clean and easy to maintain. It gives a clear distinction between errors that can be solved by the end user, the system administrator and the developer. Naming conventions and a simple set of coding guidelines ensure that helpful error messages can be easily derived from the code.

Most code examples work with Python 2.6+ and Python 3.x, on a few occasions minor differences are pointed out.

Topics covered are:

1. Introduction to error handling in Python
    - What are errors?
    - How to represent errors in Python
    - Detecting errors
    - Delegating errors to the caller
    - clean resource management
2. Principles of solution oriented error handling
    - responsibilities between user, admin and developer
    - when to use raise or assert
3. Error messages
    - What are "good" error messages
    - How to derive error messages from the source code
    - Adding context to the error
    - How to report errors to the user
4. Solution oriented usage of Python's exception hierarchy
    - admins fix `EnvironmentError`
    - users fix `DataError`
        - representing `DataError`
        - converting exceptions to `DataError`
    - developers fix everything else
    - special Python exceptions not representing errors
5. Template for a solution oriented command line application
6. Best practices for `raise` and `except`
    - When to use `raise`?
    - When to use `except`?

This talk is a translation of a German [talk](https://github.com/roskakori/talks/tree/master/pygraz/errorhandling) given at the PyGRAZ user group and in a (slightly depythonized variant) the Grazer Linux Tag 2013 ([slides and video](http://glt13-programm.linuxtage.at/events/198.de.html)).
