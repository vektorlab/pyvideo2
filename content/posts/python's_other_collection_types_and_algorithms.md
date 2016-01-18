---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=7QiuxqEpq2o"'
ThumbnailUrl: 'http://i.ytimg.com/vi/7QiuxqEpq2o/hqdefault.jpg'
date: '2011-07-18'
speakers: [Andrew Dalke]
tags: [bisect, dictionaries, frozenset, heapq, learning, namedtuple, ordereddict]
---
It's impossible to use Python without learning about lists, dictionaries and
tuples, and most people have at least heard about sets. These four collection
types are so important and useful that Python has special syntax for creating
them.

Fewer people know about Python's other built-in collection data types and
algorithms. A deque supports fast appends and pops from both ends and is great
for breath-first searches, the heapq module helps you construct a priority
queue on top of lists, and the bisect module is handy for quick binary
searches of an already sorted list.

The defaultdict uses the dict **missing** hook as a better solution to
setdefault, OrderedDict is a dictionary that preserves insertion order, and
Counter is a dictionary specialized for counting hashable objects. A
namedtuple is handy if you want to support both index and attribute lookups
for the same item, and a frozenset is a hashable form of a set which can be
used as keys in a dictionary or set.

My talk will go over these 8 different classes and modules. I'll give concrete
examples of how to use them and why they are useful. The target audience is
intermediate programmers who are familiar with the Python's standard data
types and with data types in general, but who don't know all of the
functionality available in modern Python.

