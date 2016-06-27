---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=l9Le_JOwgsM'
Speakers: [Tomasz Paczkowski]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/l9Le_JOwgsM/hqdefault.jpg'
Title: 'Fun with cPython memory allocator'
date: '2014-07-25'
---
Working with Python does not usually involve debugging memory problems: the interpreter takes care of allocating and releasing system memory and you get to enjoy working on real problems. But what if you encounter such problems? What if your program never releases memory? How do you debug it?

I will tell a story of one programmer discovering such problems. The talk will take listeners on a journey of issues they can encounter, tools they can use to debug the problems and possible solutions to seek out. There will also be a brief mention of general memory management principles.

cPython uses a combination of its own allocator, `malloc`, and `mmap` pools to manage memory of Python programs. It usually is smart enough, but there are some darker corners that are not well known by an average Joe Programmer (read: me). 

There are tools that can help debug memory problems, but those are also relatively unknown, and tend to have documentation that one might find lacking. I will describe one such tool, called `guppy`, which I have found particulary helpful.
