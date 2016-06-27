---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: 'http://youtu.be/YcSRqAJ06KM'
Speakers: [Douglas Bagnall]
Tags: [talk]
ThumbnailUrl: 'http://i.ytimg.com/vi/YcSRqAJ06KM/hqdefault.jpg'
Title: 'Multimedia programming using Gstreamer (and, of course, Python)'
date: '2014-09-14'
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Douglas Bagnall:
Multimedia programming using Gstreamer (and, of course, Python)
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Sunday, 14 Sep 2014 - Track 1
http://kiwi.pycon.org/

**Audience level**

Intermediate

**Description**

Gstreamer is a multimedia framework consisting of hundreds of interchangeable elements that can be plugged together like toy train tracks to create efficient processing pipelines. This talk will show how easy it is to put together reasonably complex Gstreamer pipelines with Python, and indicate why you might want to. It covers Gstreamer 1.x and both versions of CPython.

**Abstract**

Gstreamer [1] is a mature framework for developing applications that decode, encode, play, analyse, broadcast, or otherwise manipulate audio and video streams. It is used on phones and embedded devices, all over the linux desktop [2], and in giant multimedia displays.

It is easy to create simple Gstreamer pipelines using shell one-liners, but with Python it is possible to go beyond that, dealing with multiple parallel streams and reconfiguring pipelines on the fly. Examples drawn from real life problems include interleaving several hundred audio streams into one multi-channel stream and splitting a video stream into 4 parts and sending each to a different projector for perfect syncronisation.

It is also possible to write a Gstreamer plugin in Python, which will be briefly touched on.

[1] http://gstreamer.freedesktop.org/
[2] http://gstreamer.freedesktop.org/apps/

**Slides**

https://speakerdeck.com/nzpug/douglas-bagnall-multimedia-programming-using-gstreamer-and-of-course-python
