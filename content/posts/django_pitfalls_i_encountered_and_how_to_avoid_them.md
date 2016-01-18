---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/390_django-pitfalls-i-encountered-and-how-to-avoid-them.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011DjangoPitfallsIEncounteredAndHowToAvoidThem207-415.jpg'
date: '2011-03-11'
speakers: [Luke Sneeringer]
tags: [pycon, pycon2011]
---
Django: Pitfalls I Encountered and How to Avoid Them

Presented by Luke Sneeringer

Are you starting a moderate to large sized Django project? Do you need to plan
ahead and build an application that will react to unanticipated needs? This
talk covers some techniques and pitfalls I encountered in writing my first
reasonably large Django site, and what I did differently the second time I
started a project.

Abstract

When working on a company product, especially one where developers don't
always have full control over the scope and needs of the application, it's
important to plan ahead for unanticipated needs.

This talk will cover simple tricks and methods that are a small amount of work
up front, but can save you lots of time later.

PyCon Talk Outline

  1. Introduction (5m) 
    * Me! 
  2. Making Mistakes 
    * It happens. "Code quality can be measured by the number of WTFs per minute in the code review." 
    * When dealing with a big, expansive framework like Django, sometimes you just don't know that something is there. Good docs don't completely solve this...there's always going to be the thing you don't find. Similarly, sometimes you don't realize how to leverage something that you do know about until much later.  
  
My regrets with my current project aren't sweeping architectural issues. I did
most of the big stuff right. My regrets are mostly small things that, because
it was my first big project, there was this piece or that piece that I didn't
see or didn't fully appreciate, and so now I have little blocks of code that
are tougher to maintain than they need to be. End of the world? No. Worth
thinking through for next time? Yes.

  3. Some trivial things (10m) 
    * Preface: Yeah, some of these are dumb. 
    * Beginning at the beginning: Project Setup 
      * I had sys.path pointing to the directory above the project root, like the tutorial does. I wish I hadn't done that. 
      * Need to run two instances on the same box that don't share the actual codebase (e.g. a staging server)? You still can, but it's more awkward. Better to set sys.path at your project root. 
    * Dude, where's my Media class? 
      * How did I do it? First I had a magic template variable. Then I copied Form.Media 
      * Then, on a later project, I realized a block works just fine. 
    * My boss wants ____ available on every page! 
      * How did I do it? I had a method we called everywhere that took arbitrary keyword arguments... 
      * Oh, there's TEMPLATE_CONTEXT_PROCESSORS... 
        * ...if you manually use RequestContext every time! So, just do that. Always. Even if you don't need it. 
        * I want .select_related('something') every time! 
        * ...so I typed it! A lot. 
        * Oh, that can be done by overriding def queryset on the manager class? That's easier to maintain... 
          * ...but make sure you set the flag to use it on related fields! 
    * We need sample data for so-and-so, such-and-such... 
      * Disclaimer: This one actually isn't mine; my boss did it. But, it's amusing, and worth mentioning. 
      * We needed sample data so my boss could preview themes...so he set up a second database, put in fake data, and hard-coded it in the app-wide (not server-specific) settings.py. 
        * Copied the entire DB structure...at the time. But it changes. 
        * Oh, and the unit testing framework didn't appreciate it, either. 
      * Fixtures are the right way (and sooner or later I'll get this fixed...it's still there). 
        * (space reserved for my stumbling upon something else silly, and hopefully humorous, that I did wrong) 
          1. How to avoid missing trivial things? 
    * Read the documentation. Over and over. 
    * Become familiar with the Django code. 
  4. A non-trivial thing: Forms (10m) 
    * Django forms can do anything...given sufficient shenanigans. Always do it the Django forms way; your life will be easier. 
    * Forms and ModelForms are static, and I needed dynamic choices on a form... 
      * ...so I just ditched newforms 
      * But wait, this is Python. A trivial function that calls the metaclass can solve this problem! 
        * This looks complicated, but it's not. Walk through how to do it. 
        * It's quite maintainable, and you get all the other bells and whistles. 
  5. Questions? (5m)

