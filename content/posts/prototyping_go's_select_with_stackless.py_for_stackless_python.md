---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/438_prototyping-go-s-select-with-stackless-py-for-stackless-python.mp4
Speakers: [Andrew Francis]
Tags: [csp, go, greenlets, pycon, pycon2011, pypy, stackless]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011PrototypingGosSelectWithStacklesspyForStackless735.png'
Title: '"Prototyping Go''s Select with stackless.py for Stackless Python"'
date: '2011-03-11'
---
Prototyping Go's Select with stackless.py for Stackless Python

Presented by Andrew Francis

Showing how to use Python to prototype powerful concurrency features for
Stackless Python. We do want you to try this at home.

Abstract

Google’s introduction of the Go language raised eyebrows in the Stackless
Python community. Although very different languages, Go and Stackless Python’s
concurrency model share a common ancestor: the Bell Labs family of languages
(i.e., Newsqueak, Limbo). The common feature are channels: a synchronous
message passing mechanism based on Tony Hoare’s Communicating Sequential
Processes (CSP).

Both Go and Python have channels. However with the select language statement,
Go has the ability to wait on multiple channels simultaneously. Select greatly
simplifies many concurrent programming problems. Stackless Python does not
have this feature. Other channel based languages also feature powerful
concurrency constructs. How hard would these constructs be to implement for
Stackless Python?

This talk explores the prototyping potential of stackless.py, the PyPy's
framework's implementation of Stackless Python. The beauty of stackless.py is
that it is written in Python and implements much of Stackless Python's API!
The "case study" involves prototyping Go's select in stackless.py before
reimplementing select in C based Stackless Python.

During this talk, it will be shown how stackless.py can be used with CPython
and the greenlet package (no need to install another Python). The audience
will also get an in depth look at how channels are implemented. Channels are
at the heart of Stackless Python's message based concurrency model. Finally
the audience will gain insights into future directions of Stackless Python.

