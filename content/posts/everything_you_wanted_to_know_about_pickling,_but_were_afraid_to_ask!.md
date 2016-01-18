---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/384_everything-you-wanted-to-know-about-pickling-but-were-afraid-to-ask.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011EverythingYouWantedToKnowAboutPicklingButWere385.png'
date: '2011-03-11'
speakers: [Richard T. Saunders]
tags: [pickling, pycon, pycon2011, serialization]
---
Everything You Wanted To Know About Pickling, But Were Afraid To Ask!

Presented by Richard T. Saunders

Serializing data structures (in Python-speak "pickling") to save to
disk/socket is an important tool for the programmer: We will discuss how the
pickling protocols (0,1,2, and 3) work as well as real-world issues (gotchas,
backwards-compatibility, etc). We will concentrate on the basics of this
stack-based protocol: what it looks like, how to encode/decode, speeds of
different implementations.

Abstract

The Pickling Protocols are a fundamental tool for saving state.

We will discuss the differences between text serialization and Python pickling
(as well as marshalling, and simple bit-blitting).

We will spend a little time discussing history: why there is a cPickle and
pickle module in 2.x and only pickle in 3.x., and why there are 4 different
protocols: 0,1,2 and 3.

We will then dive right in and look at how the stack-based protocol works. We
will concentrate on the basics (the stack-based machine), as all the protocols
adhere to this basic model, but tend to discuss the more recent protocols and
their differences. We will also discuss how the memoization scheme works.

We will show some simple examples and then build to more complex examples.

We will also discuss the relative speeds: the different protocols (text,
0,1,2,3) and the different implementations (Python, Boost, PicklingTools,
IronPython?, PyPy? Unladen Swallow?).

We will end with some real-world advice and some gotchas to watch out for
(32-bit vs. 64-bit, different versions of Python serialize differently, etc.).

