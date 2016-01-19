---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/420_the-data-structures-of-python.m4v
Speakers: [Alex Gaynor]
Tags: [abc, datastructures, dequearray, dict, ducktyping, frozenset, list, namedtuple,
  ordereddict, orderedset, pycon, pycon2011, set, tuple]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011TheDataStructuresOfPython246.png'
Title: '"The Data Structures of Python"'
date: '2011-03-11'
---
The Data Structures of Python

Presented by Alex Gaynor

Any Python programmer knows about the major builtin data strcutres, lists,
dicts, tuples, but do you always remember when you're supposed to use them? Do
you know about all the cool data structures hidden in the standard library?
This talk will be a review of the characteristics of the different data
structures, and a tour of idiomatic ways to use some of the structures in the
standard library.

Abstract

First, as a note this talk borders between survey and discuss in depth. For
each data structure I want to cover their implementation, performance
characteristics, and idiomatic usage (e.g. tuples vs. lists), a lot of them
have similar implementations so idiomatic usage will dominate for some of
them.

  * The builtins (10 minutes) 
    * lists 
      * Ordered collections of any type of objects 
      * Mutable 
      * Implemented as an array of pointers 
    * tuples 
      * Ordered collections of any type of objects 
      * Immutable* 
      * Implemented as a fixed-length array of pointers 
    * dicts 
      * Unordered mapping of hashable objects to any objects 
      * Mutable 
        * Why no immutable variant
      * Implemented as an open-addressed hash table. 
    * sets 
      * Unordered collection of hashable objects 
      * Mutable 
        * frozenset
      * Implemented as an open-addressed hash table. 
  * The Standard Library (10 minutes) 
    * OrderedDict 
      * Ordered mapping of hashable objects to any objects 
      * Mutable 
      * Implemented as a dict with a doubly-linked list running through it. 
    * deque 
      * Ordered collection of any type of objects 
      * Mutable 
      * Implemented as an unrolled, doubly-linked list 
    * namedtuple 
      * Ordered collection of any type of objects, *also* addressable by name. 
      * Immutable 
      * Implemented as a tuple with extra properties 
    * array 
      * Like a list... but limited to "primitve" types. 
  * Performance characteristics. 
  * Writing your own (5 minutes) 
    * Abstract Base Classes 
      * Duck typing 
        * Why would you want to use them!
      * What's available. 
    * OrderedSet 
      * An ordered collection of hashable objects 
      * Mutable 
      * Implemented as a set with a doubly-linked list running through it. 
  * Questions (5 minutes) 

