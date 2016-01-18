---
Category: 'DjangoCon 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/djangocon-2010/65_teaching-an-old-pony-new-tricks-maintaining-and-updating-an-aging-django-project.flv
ThumbnailUrl: 'http://a.images.blip.tv/Robertlofthouse-TeachingAnOldPonyNewTricksMaintainingAndUpdatingAnAgin531-41.jpg'
speakers: [Shawn Rider]
tags: [djangocon, djangocon2010, maintenance, updating]
---
Teaching an Old Pony New Tricks: Maintaining and Updating an Aging Django
Project

Presented by Shawn Rider

PBS began development on its first Django project in 2006 using Django 0.96.
PBS TeacherLine launched in 2007 and continues to run today. This talk will
discuss the process for designing the PBS TeacherLine codebase, how new
advanced features were added over the years, and pitfalls you can avoid when
planning projects for longevity and easy maintenance.

Abstract

PBS chose Django after seeing a presentation by Jacob Kaplan-Moss and Adrian
Holovaty at OSCON 2006. That Fall, PBS Education began work on a new version
of the PBS TeacherLine website. The site most users see when they visit PBS
TeacherLine is essentially a brochure and catalog that allows educators to
purchase seats in online professional development courses. However, behind the
scenes is an administrative infrastructure that allows over 50 PBS stations
and PBS national staff members to administrate hundreds of course sections and
over ten thousand learners every year. There are robust features for
accounting, reporting, student and staff management just to name a few.

The TeacherLine website was initially written using Django 0.96. The site is
currently running Django 1.2 and has had major upgrades made to some of the
core systems including the implementation of a robust message queue solution
to handle the most intense administrative functions. Over the past four years,
the PBS Education Technology Team has learned many lessons about system
design, best practices, handling upgrades, and creating Django-based code that
is flexible and easy to maintain.

In this discussion we will look at some of the more interesting points in the
history of PBS TeacherLine, including design patterns, workarounds that were
eventually made obsolete by improvements in the Django framework, and the
process of iteratively improving functionality and features. We will discuss
successes and failures, including the pitfalls we avoided and (perhaps more
interestingly) those we did not.

