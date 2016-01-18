---
Category: 'PyCon AU 2013'
Copyright: 'CC-BY-SA'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=Hv2pl7B1pZw"'
ThumbnailUrl: 'http://i1.ytimg.com/vi/Hv2pl7B1pZw/hqdefault.jpg'
date: '2013-07-06'
speakers: [Erik van Zijst]
tags: []
---
This talk explores the challenges of ensuring responsiveness of applications under varying conditions like suddenly increased load, code regressions and problematic user data that reveal code paths with unusually high time complexity.

I'll be looking at interrupt-driven techniques to help bring the 95 percentile of the response times of your application closer to the (usually much lower) mean.

In this talk, we'll go beyond traditional tricks like caching, sharding and data denormalization and instead look at tools that can interrupt execution of overly expensive code paths, such that you can guarantee an upper bound in response time.

Interruptingcow and django-timelimit will be some of the tools that will be covered in this talk.

The context for most of this is web applications, and I'll be drawing many examples from our ongoing experiences with running and scaling Bitbucket, which is entirely written in Python.

Having said that though, many of the tools and techniques demonstrates will apply just as well to other types of applications and situations.
