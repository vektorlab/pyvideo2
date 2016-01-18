---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/386_running-django-apps-on-google-app-engine.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011RunningDjangoAppsOnGoogleAppEngine570.png'
date: '2011-03-11'
speakers: [Wesley J. Chun]
tags: [django-nonrel, gae, googleappengine, pycon, pycon2011]
---
Running Django Apps on Google App Engine

Presented by wesley chun

In the past, Django users couldn't run apps unmodified on Google App Engine.
Some tools helped with integration but required you to change your data
models. Django-nonrel removes this requirement letting you run native Django
apps on App Engine with only config changes if you bear in mind its
restrictions like no JOINs. In this talk, we'll discuss Django-nonrel &
porting App Engine apps to Django.

Abstract

Previously, Django users could not get their apps to run unmodified on Google
App Engine, the cloud application-hosting platform. Older tools like "the
Helper" and "the Patch" required a change to the data models as well as
perhaps integrating additional tools into the application source tree. The
creators of the Patch realized how cumbersome this is and created a
replacement for all of these older tools.

Django-nonrel allows users to run pure Django apps on App Engine with only
minor configuration changes. It basically enables Django's ORM to operate on
top of non-relational databases (in addition to preserving its ability to
support standard relational DBs), one of which is Google App Engine's
Datastore. (MongoDB is another.)

What this means that current Django users can now use their existing knowledge
to write apps for App Engine as long as they keep App Engine restrictions in
mind, e.g., no JOINs. Projects written in this manner will work without any
modifications other than changing the configuration settings. On the other
side, App Engine developers now have an alternative to the '"webapp" framework
that comes with its SDK. You can now leverage the power of a full web
framework like Django and still enjoy the flexibility and scalability of App
Engine. In this talk, we'll discuss Django-nonrel, and how to port App Engine
apps from webapp to pure Django to run on App Engine using Django-nonrel.

