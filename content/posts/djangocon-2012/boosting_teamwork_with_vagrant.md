---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=DsYVx-mh3NE'
Speakers: [Julien Phalip]
Tags: [django, vagrant]
ThumbnailUrl: 'http://i.ytimg.com/vi/DsYVx-mh3NE/hqdefault.jpg'
Title: 'Boosting teamwork with Vagrant'
date: '2012-09-06'
---
In this talk I will present Vagrant, a free open-source tool facilitating the
manipulation of virtualized environments, and how it may benefit the
development of Django applications. This talk is aimed at Django developers of
all levels who are interested in getting an overview of the great
possibilities Vagrant offers to support teamwork and quality assurance.

One major benefit of using Vagrant is with on-boarding. Previously, when new
developers joined a project, it could take hours or days for them to correctly
set up their development environment and install all the projects'
dependencies (the correct version of Python, the virtualenv, the database
server, the caching engine, etc.). With Vagrant, combined with provisioning
tools like Chef or Puppet, it is now possible to easily create a virtual
machine with all the right dependencies properly pre-installed and pre-
configured to allow anyone to be fully operational and ready to contribute to
the project in a matter of minutes.

Another major benefit of Vagrant is that it gives the opportunity to create a
working environment for all developers that closely matches that of the
production server. This in turn allows to anticipate potential issues when new
code and resources eventually get deployed live.

In this talk, I will present some key functionalities and workflows around the
use of Vagrant: - installing Vagrant and Virtualbox. - creating a new virtual
machine. - provisioning a virtual machine with basic requirements. - sharing
virtual machine specifications with team members.

This talk will include a brief introduction to Chef and Puppet. It will also
include multiple practical tricks like accessing the VM's database server from
the host's machine, setting up useful shell aliases or automatically
activating the virtualenv when launching the VM.
