---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=y420yZMRdLw'
Speakers: [Petr Viktorin]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/y420yZMRdLw/hqdefault.jpg'
Title: 'The Magic of Attribute Access'
date: '2014-07-22'
---
The first part of this talk will describe what exactly happens when you
read or write an attribute in Python.

While this behavior is, of course, explained in the Python docs,
more precisely in the [Data model][1] section and [related][2] [writeups][3],
the documentation gives one a "bag of tools" and leaves combining them
to the reader.

This talk, on the other hand, will present one chunk of functionality,
the attribute lookup, and show how its mechanisms and customization
options work together to provide the flexibility (and gotchas) Python provides.
The topics covered will be:

* method resolution order, with a nod to the C3 algorithm
* instance-, class-, and metaclass-level variables
* `__dict__` and `__slots__`
* data/non-data descriptors
* special methods (`__getattr__`, `__getattribute__`, `__setattr__`, `__dir__`)


In the second part of the talk, I will show how to use the customization
primitives explained before on several interesting and/or useful examples:

* A proxy object using `__getattr__`
* Generic desciptor - an ORM column sketch
* the rudimentary `@property`, method, `staticmethod` reimplemented in
  pure Python (explained [here][2] and elsewhere), which lead to
* SQLAlchemy's [`@hybrid_proprerty`][4]
* Pyramid's deceptively simple memoizing decorator, [`@reify`][5]
* An ["Unpacked" tuple properties][6] example to drive home the idea that
  descriptors can do more than provide attribute access
  (and mention weak dicts as a way to non-intrusively store data on an object)


(These are subject to change as I compose the talk. Also some examples may
end up interleaved with the theory.)

Hopefully I'll have time to conclude with a remark about how Python manages to be
a "simple language" despite having these relatively complex mechanisms.


[1]: http://docs.python.org/3/reference/datamodel.html
[2]: http://docs.python.org/3/howto/descriptor.html
[3]: https://www.python.org/download/releases/2.3/mro/
[4]: http://docs.sqlalchemy.org/en/rel_0_9/orm/extensions/hybrid.html
[5]: http://docs.pylonsproject.org/projects/pyramid/en/latest/api/decorator.html
[6]: https://gist.github.com/encukou/9789993