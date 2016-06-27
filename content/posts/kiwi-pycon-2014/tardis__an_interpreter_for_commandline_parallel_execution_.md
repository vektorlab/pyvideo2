---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: 'http://youtu.be/Kf8Dy8Dt6YM'
Speakers: [Alan McCulloch]
Tags: [talk]
ThumbnailUrl: 'http://i.ytimg.com/vi/Kf8Dy8Dt6YM/hqdefault.jpg'
Title: 'tardis - an interpreter for command-line parallel execution '
date: '2014-09-13'
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Alan McCulloch:
tardis - an interpreter for command-line parallel execution
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Saturday, 13 Sep 2014 - Track 2
http://kiwi.pycon.org/

**Audience level**

Intermediate

**Description**

This talk is about simplifying the command line interface to local or cluster based parallel computing.

**Abstract**

Ideally the user of a command shell would be unaware whether their commands were executed as a single process on the local machine, or as many concurrent processes on either their local machine or a remote cluster, apart from the reduced time taken to complete the command if executed as concurrent processes. We have developed an approach which we call “command conditioning” in which the user marks up a command with hints to the interpreter which are used to transform the marked-up command into “(re)conditioned” native shell commands which the interpreter then launches concurrently and monitors, collects and collates output and termination status. We have implemented an initial python based command-conditioning interpreter called tardis. We describe tardis, give examples of the class of compute tasks for which it is suited, and briefly outline key compute-cluster design characteristics which support this approach. We also touch on future work such as potential integration with Galaxy, a popular python based workflow system.

**Slides**

https://speakerdeck.com/nzpug/alan-mcculloch-tardis-an-interpreter-for-command-line-parallel-execution
