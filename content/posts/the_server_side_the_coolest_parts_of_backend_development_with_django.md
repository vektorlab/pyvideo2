---
Category: 'DjangoCon AU 2013'
Copyright: 'CC-BY-SA'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=nTMupredqR0"'
ThumbnailUrl: 'http://i1.ytimg.com/vi/nTMupredqR0/hqdefault.jpg'
date: '2013-07-05'
speakers: [Tom Eastman]
tags: []
---
There are few feelings more sweet than being a web-app backend developer, and knowing that the vaguaries and frustrations of front-end design, Javascript inconsistencies, and web-browser quirks are "Someone Else's Problem". 

The backend developer, instead, has just three goals: Make the system lightning fast and infinitely scalable; ensure its absolute security and impregnability; and guarantee its absolute correctness, stability, and general perfection in the face of all input at all times.

I'll take that over having to debug CSS rendering quirks any day of the week.

In this talk I'll cover these three goals and how Django helps make each one achievable, including a tour of some of the lesser known features of the framework, such as:

 - Magic tricks you can do with Django's caching framework beyond the naive "cache this page", and its ability to take advantage of the browser's own cache in marvellous ways.
 - Taking Django's testing framework to its logical (and illogical) extremes. Including clever uses of selenium and webdriver to run unit tests, integration tests and even Javascript tests.
 - Considerations of Django use and web security. Including the sorts of things Django does a great job of protecting you from, and the things where your own due dilligence will always be required.