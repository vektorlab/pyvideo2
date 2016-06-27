---
Category: 'PyCon US 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2010/307_mastering-team-play-four-powerful-examples-of-composing-python-tools-184.ogv
Speakers: [Raymond Hettinger]
Tags: [bisect, dequeues, frozensets, heapq, lists, pycon, pycon2010, sets, sorts,
  weakreferences]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2010MasteringTeamPlayFourPowerfulExamplesOfComposin150.png'
Title: 'Mastering Team Play: Four powerful examples of composing Python tools (#184)'
date: '2010-02-19'
---
Mastering Team Play: Four powerful examples of composing Python tools

  
Presented by Raymond Hettinger

  
Starts with a quick review of the performance characteristics of major
individual tools in Python: bisect, heapq, lists, deques, sets, frozensets,
class structures, sorts, and weakreferences. Show how these tools can be
powerfully combined to create elegant solutions to four hard problems.

  1. Random sampling: when one data structure isn't enough. Discuss how the nature of the problem dictates when to use one of two alternate data structures. 
  2. Ordered dictionaries: with the right compostion of dictionaries, linked lists, and weak references, a dictionary can remember its insertion order without any impact on its big-Oh running times. 
  3. NFA to DFA conversion. The classic, but difficult, algorithm for lexical analysis becomes simple when composing Python's dicts and frozensets. 
  4. Running median: the obvious approaches are horribly slow. The problem centers around how to efficiently maintain sorted data while advancing a large sliding window one value at a time. A list of deques provides a dramatic and scalable improvement in running time. 
