---
Category: 'PyCon Italia 2015'
Copyright: ''
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=YFY7XH4PtPw"'
Speakers: [Cesare Di Mauro]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/YFY7XH4PtPw/maxresdefault.jpg'
Title: '"Writing an 8086 emulator"'
date: '2015-06-09'
---
An 8086 emulator written in Python is presented. The talk gives a brief introduction to the 8086 architecture, the pitfalls on emulating it, and the challenge to have a working model ready to be quickly ported in C (which is the final goal of the project). Some classes are presented that try to “mimic” the C memory pointers handling, to make the port easier. A set of APIs is shown, which are exposed to the emulator “consumers” (applications, drivers, or kernels). Finally, some words are spent about how testing is done and can be reused by the C version as well.