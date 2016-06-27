---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/396_an-outsider-s-look-at-co-routines.mp4
Speakers: [Peter Portante]
Tags: [concurrence, coroutines, gevent, greenlets, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011AnOutsidersLookAtCoroutines790-929.jpg'
Title: 'An outsider''s look at co-routines.'
date: '2011-03-11'
---
An outsider's look at co-routines.

Presented by Peter Portante

Let's take an outsiders look at coroutines, the underlying concept used by
greenlets. First we'll define what they are conceptually, and show some
typical use cases. Then we'll take a look at a sampling of the implementations
out there to see what they are actually doing to implement the concept.
Finally, we'll show their pluses and minuses, and highlight some features of
packages that use them.

Abstract

Talk outline:

  * Define what a coroutine is 
    * Coroutine state not known to operating system 
    * Difference between a thread or process 
    * What state is required for tracking 
  * Show how coroutines are used 
    * gevent example 
    * concurrence example 
  * Review two implementations 
    * Greenlets 
    * Python based co-routines using generators 
  * Advantages/Disadvantages 
  * Differentiating features of packages that use them 
    * Concurrence 
    * Gevent 
    * Eventlets 
