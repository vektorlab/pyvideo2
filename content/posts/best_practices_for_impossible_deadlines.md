---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/391_best-practices-for-impossible-deadlines.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011BestPracticesForImpossibleDeadlines540-981.jpg'
date: '2011-03-11'
speakers: [Christopher Groskopf]
tags: [beeswithmachineguns, bestpractices, casestudy, pycon, pycon2011]
---
Best Practices for Impossible Deadlines

Presented by Christopher Groskopf

At the Chicago Tribune we develop, test, and deploy production web
applications on schedules that range from two hours to two months. This talk
will discuss the tools and techniques that allow us to make our deadlines,
including automated deployments, frameworks, just-in-time testing, and more.
Attention will be paid to [http://github.com/newsapps/beeswithmachineguns](htt
p://github.com/newsapps/beeswithmachineguns) and the problems they solve.

Abstract

On my first day at the Chicago Tribune I was given a CSV of data about
defoliant spraying in Vietnam and told to build this: Agent Orange. What
followed was one of the most stressful and difficult weeks of my life, during
which I learned an incredible amount about web development. I had to stop
thinking about databases and start thinking about serialized JSON structures
stashed on S3; stop thinking about building tools and start thinking about
mashing up tech that was never designed to be married (in this case Simile
Timeline and Google Maps); stop thinking about idealistic development
practices and start thinking about getting a working product out the door. In
short: I had to rewire my brain for news.

This talk will go in-depth on deadline-oriented strategies that I've learned
in a year of building news applications. Some of these revolve around specific
technologies, like fabric for single-keystroke deployments or Varnish for
caching, but most will be matters of practice, like what to test when you have
no time for testing or how to avoid (yes, avoid!) database migrations.

They say Django is "the web framework for perfectionists with deadlines." This
is their Art of War.

Talk outline:

  * An anecdote: Agent Orange 
  * We can't have nice things (or best practices) 
  * Low-hanging fruit: staging environment, git branches, PEP8. 
  * Only build it once: Iterations, interviews and stakeholders 
  * Salvage, share and steal [code] 
  * Keeping track: Be a ticketing warrior 
  * Tools improve faster than you do: iterate your stack 
  * Single-keystroke deployment (fabric) 
  * Migrations are hard: Building read-only apps 
  * Don't serve that: Using S3 for hosting 
  * Caching > optimization (varnish) 
  * Know your load limits (beeswithmachineguns) 
  * Configuration-as-application: application frameworks (maps, tables) 
  * Pair programming > functional testing > unit testing 
  * except UseWordpress, e: print "No, really" 

Sites that will be used as examples:

  * Agent Orange 
  * Burr Oak Memorial 
  * Census 2010: Cook county participation rates map 
  * Area judges and supervision rates of speeders table 
  * RedEye Homicide Tracker 
  * Chicago Tribune Elections Center 
  * 2010 Illinois School Report Cards 
  * TribLocal 

