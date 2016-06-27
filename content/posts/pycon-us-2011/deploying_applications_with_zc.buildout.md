---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/426_deploying-applications-with-zc-buildout.mp4
Speakers: [JIm Fulton]
Tags: [deployment, pycon, pycon2011, zc.buildout]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011DeployingApplicationsWithZcbuildout710.png'
Title: 'Deploying Applications with zc.buildout'
date: '2011-03-11'
---
Deploying Applications with zc.buildout

Presented by JIm Fulton

This talk described using zc.buildout for application deployment to production
environments. It presents building self-contained source releases, and using
these to create RPM distributions. It shows how to use buildout to configure
services, including web servers, cron jobs, monitoring and so on. Finally, it
presents ongoing efforts to deploy applications that span many machines.

Abstract

We build and deploy large Python applications for our customers. These
applications are built from many component parts including Python packages and
non-python applications and tools. Assembling these pieces can be a tedious
and error-prone process. The zc.buildout (Buildout) package was developed to
automate this process.

As our use of buildout has matured, we've integrated it with system packaging
tools and developed techniques for managing software deployemnt and service
configuration. I'll provide a detailed description of the techniques and tools
used.

Outline:

  * Buildout 
    * Motivation 
    * History 
    * Configuration files 
    * Recipes 
  * Deployment pholisophy: keeping software and service configuration separate 
  * System Packaging 
    * Making self-contained source releases (tar balls) 
    * Creating system packages from source releases with RPM 
  * Service configuration -- system build outs 
    * Scope: Python processes, cron, log rotation, run scripts, monitoring, etc. 
    * Place files in "standard" locations. 
    * Run by root 
    * examples 
  * Meta recipes 
    * Goal: provide only essential information. 
    * Recipes provide basic level of abstraction. 
    * Buildout provides basic tools to build on these abstractions, but these tools only scale so far. 
    * Buildout configuration language is *not* a programming language. 
    * Meta-recipes provide a much more powerful way to build high-level abstractions over basic recipes. 
  * Next step: Make me a ... 
    * Model based definition of complete systems spanning multiple hosts with interlocking services 
    * Automatic management of resources 
    * Implemented with ssh, system packaging tools (e.g. yum) and buildout-based tools. 
    * Four levels of abstraction 
    * Current status 
