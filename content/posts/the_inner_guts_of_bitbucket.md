---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=2ll2ER3wpus"'
ThumbnailUrl: 'http://i.ytimg.com/vi/2ll2ER3wpus/hqdefault.jpg'
date: '2014-07-24'
speakers: [Erik van Zijst]
tags: []
---
This talk is about Bitbucket's architecture. Leaving no stone unturned, I'll be covering the entire infrastructure. Every component, from web servers to message brokers and load balancing to managing hundreds of terabytes of data.

Since its inception in 2008, Bitbucket has grown from a standard, modest Django app into a large, complex stack that while still based around Django, has expanded into many more components.

Today Bitbucket is more than 30 times bigger than at the time of acquisition almost 4 years ago and serves Git and Mercurial repos to over a million users and growing faster now than ever before.

Our current architecture and infrastructure was shaped by rapid growth and has resulted in a large, mostly horizontally scalable system. What has not changed is that it's still nearly all Python based and could serve as inspiration or validation for other community members responsible for rapidly scaling their apps.

This talk will layout the entire architecture and motivate our technology choices. From our Gunicorn to Celery and HA-Proxy to NFS.
