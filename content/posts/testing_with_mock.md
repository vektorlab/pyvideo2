---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/392_testing-with-mock.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011TestingWithMock498.png'
date: '2011-03-11'
speakers: [Michael Foord]
tags: [mock, pycon, pycon2011, testing]
---
Testing with mock

Presented by Michael Foord

mock is a Python testing library. It has the goal of making mocking in tests
brain dead simple! mock provides the Mock class and the patch decorator for
safely patching out the objects you are mocking in your tests. This talk will
cover standard mocking patterns. We'll also look at some of the newer features
in the latest release, including support for mocking magic methods.

Abstract

mock provides a core Mock class that removes the need to create a host of
trivial stubs throughout your test suite. After performing an action, you can
make assertions about which methods / attributes were used and arguments they
were called with. You can also specify return values and set specific
attributes in the normal way.

  * [http://www.voidspace.org.uk/python/mock/](http://www.voidspace.org.uk/python/mock/)
  * [http://pypi.python.org/pypi/mock/](http://pypi.python.org/pypi/mock/)

The mock module also provides a patch() decorator that handles safely patching
out the things you are mocking during your test.

We'll cover standard mocking patterns, and how mock makes them easy. We'll
also be looking at some of the newer features in the latest release, including
the magic method support that can be used (for example) for mocking out
objects used as context managers.

mock is designed for "unit test style" testing, but is used with Python
testing libraries like nose and py.test.

There will be some emphasis on how *not* to use mocking in testing, and why
'over mocking' is bad (and makes for brittle tests).

