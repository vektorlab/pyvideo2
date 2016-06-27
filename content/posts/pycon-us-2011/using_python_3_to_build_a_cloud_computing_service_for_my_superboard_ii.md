---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/443_using-python-3-to-build-a-cloud-computing-service-for-my-superboard-ii.mp4
Speakers: [David Beazley]
Tags: [pycon, pycon2011, soawesome, superboard]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011UsingPython3ToBuildACloudComputingServiceFor438.png'
Title: 'Using Python 3 to Build a Cloud Computing Service for my Superboard II'
date: '2011-03-11'
---
Using Python 3 to Build a Cloud Computing Service for my Superboard II

Presented by David Beazley

The OSI Superboard II was the computer on which I first learned to program
back in 1979. Python is why programming remains fun today. In this tale of old
meets new, I describe how I have used Python 3 to create a cloud computing
service for my still-working Superboard--a problem complicated by it only
having 8Kb of RAM and 300-baud cassette tape audio ports for I/O.

Abstract

Python 3, what good is it? Cloud computing? Bah! In this talk, I describe how
I have used Python 3 to build a distributed cloud-computing service for my
Superboard II system. Originally built in 1978, the Superboard is an obvious
candidate for cloud computing due to its extremely constrained memory (8Kb),
slow processor (a 1Mhz 6502), crippled I/O (300 baud over audio), and retro
programming environment (Microsoft Basic 1.0). The only question is how to do
it?

To answer that question, this talk consist of two main parts. In the first
part, I discuss the problem of building a communications stack between the
Superboard and a Mac using nothing but audio line-in/line-out ports--a problem
involving a tricky I/O handling, real-time audio signal processing, and the
creation of a data-link layer communication protocol. In the second part, I
discuss the creation of a distributed cloud-computing service and related
topics including messaging systems, key-value stores, map-reduce, etc.

The primary implementation language for all of this work is Python 3.
Throughout the talk, I will mention interesting Python 3 programming idioms
along with pros and cons. I'll conclude by summarizing my experience trying to
build a significant project entirely in Python 3.
