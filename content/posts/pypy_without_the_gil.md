---
Category: 'PyCon US 2013'
Copyright: 'CC'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=Q9wf63flICs'
Speakers: [Armin Rigo]
Tags: [talk]
ThumbnailUrl: 'http://i2.ytimg.com/vi/Q9wf63flICs/hqdefault.jpg'
Title: 'PyPy without the GIL'
date: '2013-03-15'
---
PyPy has a version without the Global Interpreter Lock (GIL).  It can run multiple threads concurrently.  But the real benefit is that you have other, new ways of using all your cores.  In this talk I will describe how it is possible (STM) and then focus on some of these new opportunities, e.g. show how we used multiple cores in a single really big program without adding thread locks everywhere.