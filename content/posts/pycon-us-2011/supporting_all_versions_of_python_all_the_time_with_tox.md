---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/435_supporting-all-versions-of-python-all-the-time-with-tox.mp4
Speakers: [Kumar McMillan]
Tags: [ci, hudson, pycon, pycon2011, testing, tox]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011SupportingAllVersionsOfPythonAllTheTimeWithT333.png'
Title: 'Supporting All Versions of Python All The Time With Tox'
date: '2011-03-11'
---
Supporting All Versions of Python All The Time With Tox

Presented by Kumar McMillan

This talk explains the modern techniques that every module maintainer needs to
know in order to support all major versions of Python. You probably already
have a massive test suite using a tool like nosetests, py.test, unittest, or a
custom runner. Using the tox command line tool, you'll see how to run your
tests in Python 2.x, 3.x, Jython, and whatever else in parallel.

Abstract

tox is a new tool that lets you set up isolated virtual environments to test
your module's deployment and compatibility with all major versions of Python.
It's easy to install and is flexible enough that it probably already supports
your existing test suite. With one simple command you can execute your test
suite in each version of Python, you can build its documentation with Sphinx,
and get a nice printout of the results. It has also been designed from the
ground up to integrate into continuous integration (CI) tools like Hudson.

Using practical examples, this talk will show you how to toxify your existing
test suite and trick it out with the tox.ini config file. You'll also see how
to leverage Hudson's matrix build so that each code checkin will run tests in
all versions of Python and report detailed failures.

Your app supports Python 3, right? No? Tox is the best way to develop in
parallel with 2.x and 3.x. We'll go over how to set up tox for that.

