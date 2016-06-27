---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=U_IZVEZImq4'
Speakers: [Magnus Hagander]
Tags: [cache, database, deploy, design, django, framework, web]
ThumbnailUrl: 'http://i.ytimg.com/vi/U_IZVEZImq4/hqdefault.jpg'
Title: 'Data Driven Cache Invalidation'
date: '2011-07-24'
---
In todays world, nobody (should) deploy a web application facing the internet
without having a proper caching system in place. There are many different
solutions to choose from, from manual use of memcached through framework
integrated caching to external caches like Squid or Varnish. Most modern
frameworks come with integrated functionality for at least one of these
methods, and often more than one.

However, they often relies on all traffic going through the same framework to
work properly - a caching layer in Rails is hard to share with one in Django.
This talk will show a way to break the design rules of these frameworks just a
little, and have the database help solve this problem.

This talk will use a small application written in Python using Django to
illustrate the examples, but the method is language independent.
Unsurprisingly, the database used is PostgreSQL.
