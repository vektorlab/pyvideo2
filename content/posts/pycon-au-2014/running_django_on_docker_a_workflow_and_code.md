---
Category: 'PyCon AU 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=SgL8r--p97s'
Speakers: [Alexey Kotlyarov, Danielle Madeley]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/SgL8r--p97s/hqdefault.jpg'
Title: 'Running Django on Docker: a workflow and code'
date: '2014-08-09'
---
Docker (http://docker.io) is the hot-new-thing out there for running your application in development and in production. Here at Infoxchange, we are extremely excited about how Docker allows a build-once, run-anywhere approach to moving applications from testing through to production. We are one of the first organisations to be using Docker in production on high-SLA applications.

In this talk we will present:

- a quick intro to Docker and how it solves our problems at Infoxchange;
- our interface for hosting applications on Docker ("pallet");
- how to build and develop a Python app on Docker;
- Infoxchange's Django settings module for the pallet interface;
- Forklift (https://github.com/infoxchange/docker-forklift), a tool we've developed for running and developing apps that use the pallet interface, in and out of a Docker container; and
- Extending forklift for your services.

If time permits we will try and cover the additional bonus topics:

- How to host your legacy mod_python application on Apache inside Docker with minimal changes; and
- Using Forklift to do automated full-stack integration testing of apps by spinning up containers of other apps (which we do in a container that is testing the built app that is running in a container that is our CI server... inception is possible).

The talk will be presented by Danielle Madeley and Alexey Kotlyarov.
