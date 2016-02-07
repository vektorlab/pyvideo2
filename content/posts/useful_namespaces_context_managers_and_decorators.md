---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/395_useful-namespaces-context-managers-and-decorators.mp4
Speakers: [Jack Diederich]
Tags: [contextmanagers, decorators, namespaces, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011UsefulNamespacesContextManagersAndDecorators353.png'
Title: 'Useful Namespaces: Context Managers and Decorators'
date: '2011-03-11'
---
Useful Namespaces: Context Managers and Decorators

Presented by Jack Diederich

Python has two useful conventions for "I mean it, but only here" and you can
say it with Context Managers and Decorators. Both give you the power to define
a push/pop of a resource for a set period inside a namespace, be it a function
or a level of indentation. This talk is a list of patterns that are
implemented by one or the other (including some clever functions that are
both).

Abstract

  * Decorators, formal definition. 
  * Context Managers, formal definition. 
  * Informal definition: both have the opportunity to do and then undo. - very similar to C++ RIIA "Resource Acquisition Is Initialization." - Context Managers were designed to do that but decorators are frequently just as good. 
  * Which one to use use when is all about namespaces. - Context Managers manipulate at the block level. - Function Decorators manipulate the function level. - Class Decorators manipulate at the class level. 
  * Recipes on writing decorators and context managers - Familiar examples from Django and Mock. 

