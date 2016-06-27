---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/431_dependency-management-with-puppet.mp4
Speakers: [Richard Crowley]
Tags: [dependencies, puppet, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011DependencyManagementWithPuppet645.png'
Title: 'Dependency management with Puppet'
date: '2011-03-11'
---
Dependency management with Puppet

Presented by Richard Crowley

Puppet is a configuration management tool that we'll learn to use the easy
way. We'll introduce the Puppet language and the concept of resources like
packages, files, shell commands, and more. We'll use Puppet to build our dev
environment and deploy it to production servers.

Abstract

We've all been there: religiously following the steps in some blog post for
the 47th time trying to setup a shiny new server. We thought we'd improved the
situation when we copied our Bash history into doit.sh and committed it. Then
along came Pip and requirements.txt files.

That's where most of us are today. Pip can only manage Python packages so much
of our servers' behavior is left to Lady Luck. Puppet gives us the power to
efficiently and confidently specify everything our program needs.

We'll start at square one and the concept of resources, the basic unit of
configuration management. We'll learn the Puppet language's resource syntax.
We'll talk about obvious resource types like packages and files plus less
obvious types like shell commands, users, groups, and daemons. We'll compose
resources into larger ones, declare dependencies between resources, and
accommodate differences between OS X and Linux.

These Puppet manifests can satisfy our program's dependencies on demand,
making them ideal parts of the deploy process. We'll walk through how Puppet
is used to build production environments both through tools such as Fabric and
Puppet's traditional client-server mode.

Dependency hell doesn't have to be your reality. Consistent, reliable
environments can be had with Puppet.
