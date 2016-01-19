---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: '"http://youtu.be/265Sqo7cgbM"'
Speakers: [Danny Adair]
Tags: [talk]
ThumbnailUrl: 'http://i.ytimg.com/vi/265Sqo7cgbM/hqdefault.jpg'
Title: '"The Full Monty - CI on OpenStack"'
date: '2014-09-13'
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Danny Adair:
The Full Monty - CI on OpenStack
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Saturday, 13 Sep 2014 - Track 1 
http://kiwi.pycon.org/

**Audience level**

Intermediate

**Description**

Are you continuously "integrating", or just running some unit tests inside a virtualenv?

Let's go the Full Monty with OpenStack!

Protagonists, in order of appearance: Gerrit, Jenkins, OpenStack, Puppet, Odoo (formerly OpenERP). Enjoy the ride!

**Abstract**

I'll show how we configured our CI tools to automatically build and destroy entire servers on OpenStack. We'll have Gerrit for code review, Jenkins for coordinating and monitoring the build process, OpenStack and its tools to build servers on their own subnet, Puppet for configuring said servers. The example project is an installation of Odoo (formely OpenERP) with a web server and PostgreSQL database.

At Catalyst, my team works with Odoo (formerly known as OpenERP), a modular Open Source suite of business applications. It has a very large and complex codebase and "Regression" is its middle name. It is under very active development on github, and customisations are generally brought in via plugins that override or extend default functionality. Basically, reasonable work on this requires continuous integration, it's not a luxury.

We could have a fat build server with multiple virtualenvs and multiple databases on the same PostgreSQL server, and just run some Python tests and be done with it. We could improve that with something like LXC, Vagrant etc. all happening on said build server. But why stop there - why not go all the way and create a more realistic setup? After all, another team is able to provide us with OpenStack. Let's go the Full Monty!

Let's go hog wild and create and destroy entire servers just for the purpose of testing. Let's have separate application and database servers, just like in production.

Let's also keep some servers alive for other purposes, e.g., user acceptance testing. Just sit in an IRC channel and after changes are committed for review, wait for a bot to post the URL of the newly built web server to click on. A nicely readable URL on a separate subdomain that is, of course!

As a bonus, I'll show how active upstream development on github fits into all this, and how your Ubuntu "Precise Pangolin" server can easily rehearse an upgrade to "Trusty Tahr".

**Slides**

https://speakerdeck.com/nzpug/danny-adair-the-full-monty-ci-on-openstack