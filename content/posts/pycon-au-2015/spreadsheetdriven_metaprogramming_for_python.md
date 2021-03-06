---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=DmLHqOvbG9M'
Speakers: [Javier Candeira]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/DmLHqOvbG9M/hqdefault.jpg'
Title: 'Spreadsheet-Driven Meta-Programming for Python'
date: '2015-08-04'
---
We've all had those very detail-oriented clients who are able to specify their needs very neatly, often by means of exhaustive spreadsheets. Wouldn't it be nice if we could turn these spreadsheets straight into Python code?

In this tutorial we'll use two sets of meta-programming techniques to derive Python code out of semi-formal descriptions: first, to build Django models requiring very detailed validation supplied by the client in a spreadsheet; second, to build a Python API for a hardware device, the description of which is maintained by the engineers in a spreadsheet.

For the Pycon attendance, this tutorial has both business value and technical value:

Business value because spreadsheet-driven metaprogramming allows developers to:

- respond to changes very fast by re-rendering their Python code from the modified spreadsheet descriptions.
- avoid a certain class of human errors unavoidable when transcribing the requirements by hand.
- save time which can be employed in other areas of the project, or with other clients.
- clarify ambiguous specifications by making explicit all programmer's assumptions into the code generator.

Technical value because we'll be talking about:

- api design,
- Django modeling and validation,
- consuming spreadsheets via csv dictreaders and elbow grease,
- writing partially-applied functions via custom classes with a __call__ method,
- implementing fluent apis with table-driven __getattr__ methods,
- implementing iterators with __iter__ and __next__,
- papering over some differences between Python 2 and Python 3 syntax,
- and much, much more.

We'll be doing all of it in a hands-on manner, without getting distracted by abstract discussions of Python syntax. There will be some discussions of Python syntax, but they won't be abstract. We'll always have a goal in sight.

Level:

Intermediate. You'll learn some advanced techniques, but all you need to really know in order to follow this tutorial is how lists, dictionaries, iteration and reading files work in Python. 

Requirements:

- Attendees are expected to know basic Python (see above, under "Level").
- A laptop and some knowledge of git will be useful for those wanting to follow along, but is not required. You can get a lot out of this tutorial just by watching and paying attention.
