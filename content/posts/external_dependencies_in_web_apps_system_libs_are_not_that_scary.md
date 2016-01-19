---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: '"http://youtu.be/wfDhGAMPS1g"'
Speakers: [Francois Marier]
Tags: [talk]
ThumbnailUrl: 'http://i.ytimg.com/vi/wfDhGAMPS1g/hqdefault.jpg'
Title: '"External dependencies in web apps: system libs are not that scary"'
date: '2014-09-13'
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Francois Marier:
External dependencies in web apps: system libs are not that scary
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Saturday, 13 Sep 2014 - Track 2 
http://kiwi.pycon.org/

**Audience level**

Intermediate

**Description**

Going to production is very different from setting up a development environment. We have great tools like pip and virtualenv for the latter but they lead to maintenance anti-patterns when they are used for production deployments. We don't "pip install apache" and instead leverage the QA and integration work of distro developers, so why not rely on distros for more than just the base system?

**Abstract**

Today's web applications often have a lot of external dependencies. Start off with a basic framework, sprinkle a couple of handy plugins or python modules and finish with a generous serving of JavaScript front-end libraries.

What you end up is a gigantic mess of code from different sources which follow very different release schedules and policies. Language-specific package managers can automate much of the dependency resolution and package installation, but you're on your own in terms of integration and quality assurance. Also, the minute you start distributing someone else's code with your project, you become responsible for the security of that external code.

You could of course decide to avoid the problem by writing it all yourself from scratch. Realistically though, you're not likely to go past the stage of a toy WSGI app using that approach because it's a lot of work.

This talk will examine the decision that the Libravatar [1] project made to outsource much of its maintenance burden to the distro by using system packages for almost everything.

[1] https://www.libravatar.org/

**Slides**

https://speakerdeck.com/nzpug/francois-marier-external-dependencies-in-web-apps-system-libs-are-not-that-scary