---
Category: 'Kiwi PyCon 2013'
Copyright: ''
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=W7Rv-km3ZuA"'
Speakers: [Graham Dumpleton]
Tags: []
ThumbnailUrl: 'http://i1.ytimg.com/vi/W7Rv-km3ZuA/hqdefault.jpg'
Title: '"Advanced methods for creating decorators"'
date: '2013-09-15'
---
@ Kiwi PyCon 2013 - Sunday, 08 Sep 2013 - Track 1

**Audience level**

Experienced

**Abstract**

A decorator is any callable Python object that is used to modify a function, method or class definition. A decorator is passed the original object being defined and returns a modified object, which is then bound to the name in the definition.

One would generally expect the result of applying a decorator to an object to be another object which is not readily distinguishable from the original. Naive implementations of decorators do not however preserve introspectability. This can result in callable objects having different names, appearing to have different signatures or not returning the original doc strings. This can cause problems for tools where you want to derive information about the original wrapped object such as debuggers, IDEs, documentation systems or performance monitoring software.

The use of the functools.wraps() decorator addresses some of these issues, but relies on decorators being implemented as closures. Using a closure to implement a decorator will not always work when wrapping functions where the descriptor protocol needs to be triggered to bind a function to an instance, to create an instance method, or where the function is a special method type such as a class method or static method.

A more robust decorator, and one where the decorator is able to distinguish when it is being applied to a normal function or instance method, needs to be implemented as a combination of a wrapper and a descriptor. To also be able to use this as a generic wrapper when performing monkey patching requires even more tricks.

The purpose of this talk is to walk through the various problems which arise with the more common ways of implementing decorators. It will then describe how to create a more robust generic wrapper/decorator which can be used in a wider range of scenarios than typical decorators.

**Slides**

https://speakerdeck.com/nzpug/graham-dumpleton-advanced-methods-for-creating-decorators