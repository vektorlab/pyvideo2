---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/407_continuous-deployment.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011ContinuousDeployment817.png'
date: '2011-03-11'
speakers: [Laurens Van Houtven]
tags: [cd, ci, continuousdeployment, deployment, pycon, pycon2011, softwaredevelopment,
  tdd, workflow]
---
Continuous deployment

Presented by Laurens Van Houtven

This talk is about continuous deployment practices and tools, lessons learned
from implementing it, and putting them into perspective. The goal is to give
other people tips and pointers for applying these ideas themselves.

Abstract

Continuous deployment is the practice of putting the latest revision of
software into production use all the time, as opposed to working towards
larger releases. The important difference is iteration time: whereas large
software packages produce new software in timeframes of years or months,
continuous deployment teams typically put new code into production in
timeframes of hours or less.

The practice is slowly attracting a small but growing group of loyal
followers, just like continuous integration over the past few years and test-
driven development did before that. They can be explained in terms of being
natural extensions of each other. Like TDD and CI, CD gets eyed somewhat
suspiciously (and rightfully so: skeptical analysis is great), but the
undersigned believes there's a legitimate advantage for many applications.

Many years ago, TTD and testing tools in general were mostly ad-hockery. Now,
with many different production-quality testing tools, this has become
unthinkable. Similarly, continuous integration was something other people did
for a long time, but now we have tools such as Buildbot and Hudson. Continuous
deployment is still somewhat in the early stage in terms of ready-to-use
tools, but it's likely that we'll see a similar evolution.

Here's a rough outline of what I plan to cover:

  * a short history of people developed software 
  * from the recent models to CD (sort of a working definition of CD here) 
  * when is it a good idea? pros/cons 
  * requirements & battle plan for applying CD in an existing development environment (and possibly code base) 
  * an overview of existing tools and how they work together 
  * caveat emptors, known pitfalls (deployment and recovery strategies go here, since most implementations figure out they need them after stuff blows up) 
  * questions! (hopefully lots of people who've tried or are thinking about implementing something similar -- like I said, there are a lot of people implementing it but not too many ideas being bounced around) 

