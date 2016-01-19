---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=yMyMEsOi8oY"'
Speakers: [Armin Rigo]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/yMyMEsOi8oY/hqdefault.jpg'
Title: '"Using All These Cores: Transactional Memory in PyPy"'
date: '2014-07-23'
---
PyPy is a fast alternative Python implementation.  Software Transactional Memory (STM) is a current academic research topic.  Put the two together --brew for a couple of years-- and we get a version of PyPy that runs on multiple cores, without the infamous Global Interpreter Lock (GIL).

The current research is based on a recent new insight that promises to give really good performance.  The speed of STM is generally measured by two factors: the ability to scale with the number of CPUs, and the amount of overhead when compared with other approaches in a single CPU (in this case, with the regular PyPy with the GIL).  Scaling is not really a problem here, but single-CPU performance is --or used to be. This new approach gives a single-threaded overhead that should be very low, maybe 20%, which would definitely be news for STM systems.  Right now (February 2014) we are still implementing it, so we cannot give final numbers yet, but early results on a small interpreter for a custom language are around 15%.  This looks like a deal-changer for STM.

In the talk, I will describe our progress, hopefully along with real numbers and demos.  I will then dive under the hood of PyPy to give an idea about how it works.  I will conclude with a picture of how the future of multi-threaded programming might looks like, for high-level languages like Python.  I will also mention CPython: how hard (or not) it would be to change the CPython source code to use the same approach.