---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/423_through-the-side-channel-timing-and-implementation-attacks-in-python.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011ThroughTheSideChannelTimingAndImplementationAt601.png'
date: '2011-03-11'
speakers: [Geremy Condra]
tags: [hacking, hardening, pycon, pycon2011, security]
---
Through the Side Channel: Timing and Implementation Attacks in Python

Presented by Geremy Condra

Python's dynamic nature, large standard library, and concern for beauty over
performance make it an elegant and uniquely easy to use language, but they
also cause some unique problems. In this talk we'll explore how features
ranging from dictionaries to duck typing can become security risks,
demonstrate those attacks on real Python projects, and examine how you can
protect yourself and your code.

Abstract

Over the last decade, an increasing body of evidence has accumulated
indicating that even when a system is hardened enough to provide strong
guarantees about its high-level behavior, implementation details and
especially performance properties can still provide attackers with an easy way
in. For Python, this is especially problematic: its generally high-level view
and the emphasis placed on flexibility often mean that it can be difficult to
stop attackers from gaining a foothold, while its comparatively low execution
speed increases the efficacy of wide variety of implementation and timing
attacks.

To help Pythonistas understand and cope with these problems, we've divided
this talk into two parts: in the first, we demonstrate the attacks against a
series of widely-deployed Python projects with the goal of both improving
awareness about the issue and demonstrating common weaknesses to be avoided.
The second demonstrates effective countermeasures and alternative
constructions with the goal of improving defenders' odds of spotting and
correcting these flaws in their own code.

