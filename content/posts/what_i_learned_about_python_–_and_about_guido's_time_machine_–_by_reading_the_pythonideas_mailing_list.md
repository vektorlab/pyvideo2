---
Category: 'PyCon ZA 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://archive.org/details/pyconza2014-python-ideas"'
Speakers: [David Mertz]
Tags: [pyconza, pyconza2014]
ThumbnailUrl: 'http://archive.org/download/pyconza2014-python-ideas/pyconza2014-python-ideas.thumbs/8%20What%20I%20learned%20about%20Python-_000690.jpg'
Title: What I learned about Python \u2013 and about Guido's time machine \u2013\
  \ by reading the python-ideas mailing list\
date: '2014-10-03'
---
One of the ways that changes enter the Python language is via their prior discussion on the python-ideas mailing list. Many core contributors read and contribute to this list, some do not, and a large number of other interested Python programmers also participate in the discussion. A recurring element of these fascinating discussions is that ideas which seem compelling at first blush, upon deeper discussion reveal the greater wisdom of doing things just the way Python already does. Not always, of course, but often.
A wonderful case study of this process is the innocuous seeming built-in 'sum()'. This function has an intricate history, with a great deal of dispute over just what its semantics and performance characteristics can or should be. A particular thread on python-ideas, rich with discussions of use cases and subtle semantics, led both to the creation of the 'statistics' module in Python 3.4 (which contains a "private" version of the function, 'statistics._sum()') and to a rejection of performance "optimizations" when operating over collections of collections (which may or may not seem obvious to "sum" in the first place).