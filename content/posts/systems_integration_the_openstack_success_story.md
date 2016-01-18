---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=pYzIOrAkb-A"'
ThumbnailUrl: 'http://i.ytimg.com/vi/pYzIOrAkb-A/hqdefault.jpg'
date: '2014-07-23'
speakers: [Flavio Percoco]
tags: []
---
Abstract
=======

OpenStack is a huge, open-source cloud provider. One of the main tenets of OpenStack is the (Shared Nothing Architecture) to which all modules stick very closely. In order to do that, services within OpenStack have adopted different strategies to integrate themselves and share data without sacrificing performance nor moving away from SNA.

This strategies are not applicable just to OpenStack but to any distributed system. Sharing data, regardless what that data is, is a must-have requirement of any successful cloud service.

This talk will present some of the existing integration strategies that are applicable to cloud infrastructures and enterprise services. The talk will be based on the strategies that have helped OpenStack to be successful and most importantly, scalable.

Details
======

Along the lines of what I've described in the abstract, the presentation will walk the audience through the state of the art of existing system integration solutions, the ones that have been adopted by OpenStack and the benefits of those solutions. At the end of the talk, a set of solutions under development, ideas and improvements to the existing ones will be presented.

The presentation is oriented to distributed services, fault-tolerance and replica determinism. It's based on a software completely written in python and running successfully on several production environments.

The presentation will be split in 3 main topics:

Distributed System integration
-----------------------------------

* What's it ?
* Why is it essential for cloud infrastructures?
* Existing methods and strategies

OpenStack success story
----------------------------

* Which methods did OpenStack adopt?
* How / Why do they work?
* What else could be done?

Coming Next
---------------

* Some issues of existing solutions
* What are we doing to improve that?
* Other solutions coming up