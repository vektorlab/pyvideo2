---
Category: 'Kiwi PyCon 2013'
Copyright: ''
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=HbJZu2qcC-s"'
Speakers: [Ravi Chandra]
Tags: []
ThumbnailUrl: 'http://i1.ytimg.com/vi/HbJZu2qcC-s/hqdefault.jpg'
Title: '"Fake it till you make it"'
date: '2013-09-14'
---
@ Kiwi PyCon 2013 - Saturday, 07 Sep 2013 - Track 1

**Audience level**

Intermediate

**Abstract**

In practise most of us have found testing to be much harder to achieve in the "real world". That is often because the application architecture is modular with some level of service abstraction, and the ensuing layers of code.

The premise of this talk is: do not test someone else's code. They are a good developer. They would have tested it so it must work.

Taking this perspective allows us to develop fast and compact unit tests for our application functionality while ignoring bigger picture integration issues (these can be addresses using other types of tests!). In our experience this unburdens developers so they can really practice test-driven development much more diligently.

Implementation of this approach is simplified thanks to the mock library. Mock provides a core MagicMock class that obviates the need for custom stubs throughout the code. Moreover, its supports patching specific methods, properties, and more. Mocking is used to patch calls to external code within our unit tests, since we don't need to test them, in a non-non-invasive way to our application.

**Slides**

https://speakerdeck.com/nzpug/ravi-chandra-fake-it-till-you-make-it