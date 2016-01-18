---
Category: 'PyCon US 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2010/236_django-deployment-workshop.m4v
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-DjangoDeploymentWorkshop734-407.jpg'
date: '2010-02-19'
speakers: [Jacob Kaplan-Moss]
tags: [pycon, pycon2010]
---
Django Deployment Workshop

Presented by Jacob Kaplan-Moss

So you've written a Django site... now what? Writing the application is just
the beginning; now you've got to put it into production! In this hands-on
workshop we'll walk through the creation of a full Django deployment
environment running on a cluster of (virtual) machines.

This class will introduce students to a wide variety of technologies,
including Amazon's EC2 and S3, Fabric, Varnish, nginx, mod_wsgi, memcached,
PostgreSQL, pgpool, pg_standby, and more.

By the end of the class, each student will have created an environment
featuring:

  * Multiple levels of caching and load balancing.
  * Multiple web application servers.
  * Shared media servers.
  * Redundant replicated database servers.
  * Separate caching servers.

We'll create this whole stack on Amazon EC2 virtual machines, so students will
be able to take home a complete copy of all the deployment configuration for
future review at their leisure.

Note: the example application used in this class with be a Django site, and
the class assumes at least a moderate comfort level with Django. However, the
tools and techniques apply just as well to other Python web frameworks, so
users of other tools will likely be able to follow along fairly easily.

# Intended Audience

Intermediate to advanced Django users with sites nearing or in production.
Python developers using other web frameworks will likely be able to follow
along -- see the note in the summary, above.

# Class Outline

  * Introduction: the deployment question
  * Application server: mod_wsgi
  * Database server: PostgreSQL
  * Automated deployment with Fabric
  * Multiple web servers; load balancing with nginx
  * Adding memcached
  * Database connection middleware: pgpool
  * Database redundancy: warm standby
  * Upstream caching: Varnish
  * Final load testing: how'd we do?

# Requirements

Students will need a computer and Amazon EC2 and S3 accounts, and will be
asked to familiarize themselves with the process of starting and stopping EC2
virtual machines before the class.

[http://us.pycon.org/2010/tutorials/kaplanmoss_django/](http://us.pycon.org/20
10/tutorials/kaplanmoss_django)

