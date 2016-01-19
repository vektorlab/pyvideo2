---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=elAV6aZDMvg"'
Speakers: [Stefan Schwarzer]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/elAV6aZDMvg/hqdefault.jpg'
Title: '"Support Python 2 and 3 with the same code"'
date: '2014-07-24'
---
Your library supports only Python 2, - but your users keep nagging you about Python 3 support?

As Python 3 gets adopted more and more, users ask for Python 3 support in existing libraries for Python 2. This talk mentions some approaches for giving users a Python 3 version, but will quickly focus on using the very same code for a Python 2 and a Python 3 version.

This is much easier if you require Python 2.6 and up, and yet a bit easier if you require Python 3.3 as the minimum Python 3 version.

The talk discusses main problems when supporting Python 3 (some are easily solved):

* `print` is a function.

* More Python APIs return iterators that used to return lists.

* There's now a clear distinction between bytes and unicode (text) strings.

* Files are opened as text by default, requiring an encoding to apply on reading and writing.


The talk also explains some best practices:

* Start with a good automatic test coverage.

* Deal with many automatic conversions with a one-time 2to3 run.

* Think about how your library should handle bytes and unicode strings. (Rule of thumb: Decode bytes as early as possible; encode unicode text as late as possible.)

* Should you break compatibility with your existing Python 2 API? (Yes, if there's no other way to design a sane API for Python 2 and 3. If you do it, raise the first part of the version number.)

* Try to keep code that's different for Python 2 and 3 minimal. Put code that needs to be different for Python 2 and 3 into a `compat` module. Or use third-party libraries like `six` or `future`.


Finally, the talk will mention some helpful resources on the web.