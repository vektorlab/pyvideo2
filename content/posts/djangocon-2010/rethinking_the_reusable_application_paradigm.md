---
Category: 'DjangoCon 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/djangocon-2010/51_rethinking-the-reusable-application-paradigm.flv
Speakers: [Alex Gaynor]
Tags: [djangocon, djangocon2010, modularizing, reuse, reusing]
ThumbnailUrl: 'http://a.images.blip.tv/Robertlofthouse-RethinkingTheReusableApplicationParadigm774.png'
Title: 'Rethinking the Reusable Application Paradigm'
---
Rethinking the Reusable Application Paradigm

Presented by Alex Gaynor

For the past few years the reusable application paradigm has been considered
one of the major selling points of Django, however the common wisdom about
what it means to make an application reusable isn't really accurate. This talk
is going to discuss ways to truly make your applications reusable across *any*
project.

Abstract

The common wisdom about reusable application says to do things like let your
views take arguments for things like the form class or the template name.
However, that doesn't satisfy most of the real need for extendability:
changing the business logic or altering models. This talk is going to look at
ways to combat these limitations:

  * Class based views 
  * By making everything overidable in a view you can absolutely minimize the need to "copy-paste" when changing the logic of things around. 
  * As seen in the admin. 
  * Do less 
  * brabeion 
  * Provide the absolute minimum at the model layer, and only small wrappers for the business logic users can implement their own logic to control how things happen. 
  * Related to the idea of "application frameworks". Providing the tools for others to build their logic around various helpers. 
  * Flexibility 
  * django-taggit 
  * Provide a concrete implementation, but allow swapping out of various layers. 
  * Don't like the Tag model, swap it out, want a new intermediary model, swap it out. 
  * django-registration 
  * Providing swappable backends to change behavior. 
  * Libraries 
  * django-filter 
  * django-fixture-generator 
  * django-templatetag-sugar 
  * django-compressor 
  * Providing tools for others to build around. 

By using these techniques you can develop reusable application that work
beyond any single use case. Of course there are cases where you don't need any
of these, and just need something that fits "traditional" reusable application
paradigm, so this talk will cover when that works as well.
