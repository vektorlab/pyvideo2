---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/422_units-need-testing-too.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011UnitsNeedTestingToo863.png'
date: '2011-03-11'
speakers: [Gary Bernhardt]
tags: [pycon, pycon2011, pyunit, testing, unittests]
---
Units Need Testing Too

Presented by Gary Bernhardt

Python's long history of testing has focused primarily on integration- and
system-level tests: slow-running tests executing lots of code. These are a
great start, but many of them can be transformed into unit-level tests. True
unit tests are orders of magnitude faster (about 1ms each), providing quicker
feedback and better failure localization. We'll look at why and how to write
them.

Abstract

Python has a wonderful legacy in testing: PyUnit has been in the standard
library since March, 2001, and it was already a year old by then. We adopted
browser driving quickly, and we do it at huge scale with great test
parallelization infrastructure.

Big tests aren't everything, though. In the Python world, true unit tests are
somewhat rare, and even most tests written with the unittest library are
integration tests. These tests are slow to execute and don't localize failure
as well as smaller, focused tests. They leave us with two options: either run
them rarely, sacrificing feedback, or run them often, sacrificing speed.

Writing true unit tests removes that particular trade-off. When your tests
execute in a millisecond each, you can afford to run a thousand of them every
time you save a source file. This talk will discuss what unit tests really
are, why they matter, and how to write them in Python.

