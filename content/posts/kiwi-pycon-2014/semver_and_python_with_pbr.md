---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: 'http://youtu.be/6hjg-Uia5AU'
Speakers: [Robert Collins]
Tags: [talk]
ThumbnailUrl: 'http://i.ytimg.com/vi/6hjg-Uia5AU/hqdefault.jpg'
Title: 'Semver and Python with PBR'
date: '2014-09-13'
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Robert Collins:
Semver and Python with PBR
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Saturday, 13 Sep 2014 - Track 1
http://kiwi.pycon.org/

**Audience level**

Novice

**Description**

PBR is a setuptools plugin which OpenStack developed to provide simple and consistent minimal-boilerplate build definitions for its projects. Semantic versioning provides simple and robust rules for deciding on version numbers, and PBR will soon be able to manage the entire process of version number assignment in a project... and more.

**Abstract**

PBR is a setuptools plugin which OpenStack developed to provide simple and consistent minimal-boilerplate build definitions for its projects. Now used by all the OpenStack projects, PBR provides integration glue for core features:

 - testing
 - binary package creation for Linux distributors
 - inclusion of files in tarballs
 - changelog and authors file creation
 - pypi summary creation
 - version number creation
 - sphinx doc stub creation and manpage enablement
 - unified requirements management
 - for both easy-install and pip with single-file control

The most interesting part is the version number creation, since coming up with the right version number can be a contentious discussion in some projects. Semver provides simple and robust rules for deciding on version numbers, and I'm in the middle of implementing automation for these in PBR itself, with integration glue to export them in PEP-440, dpkg and rpm format. The only dependencies PBR has are git + a recent pip, so this should be useful for many attendees - and while PBR is an OpenStack invention we're very interested in making sure its useful and reliable for anyone that wants to use it.

**Slides**

https://speakerdeck.com/nzpug/robert-collins-semver-and-python-with-pbr
