---
Category: 'PyCon AU 2012'
Copyright: 'http://www.youtube.com/t/terms'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=8fB2qY8s2i4"'
Speakers: [Ryan Kelly]
Tags: [WebTest]
ThumbnailUrl: 'http://i.ytimg.com/vi/8fB2qY8s2i4/hqdefault.jpg'
Title: '"The Lazy Dev''s Guide to Testing Your Web API"'
date: '2012-08-21'
---
Do you enjoy writing test cases for your web application? If so then this may
not be the talk for you. I'm going to show you how to make a single test suite
perform triple testing duty, so you can get on with writing the fun stuff.

First, I'll show you how to use WebTest to construct a simple functional
testsuite for your application. By running in-process against a WSGI callable,
the tests can be fast and light enough to form part of your regularly-executed
suite.

Second, we'll use WSGIProxy to turn this into a deployment/acceptance test
script that you can point at a real live server to verify its behaviour. Run
this after every deployment to make sure you haven't broken something in the
wild.

Finally, we'll connect the suite to FunkLoad and pummel the server with a
distributed barrage of tests, to see how it copes under pressure.

