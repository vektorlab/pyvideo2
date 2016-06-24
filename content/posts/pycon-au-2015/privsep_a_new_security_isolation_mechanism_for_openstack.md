---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=0FOQB4PZVe0'
Speakers: [Angus Lees]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/0FOQB4PZVe0/hqdefault.jpg'
Title: 'Privsep: A New Security Isolation Mechanism for OpenStack'
date: '2015-08-16'
---
OpenStack listens to requests over the network, and (when appropriate) performs operations on the host that require root superpowers.  Following best-practice design, most of the code runs as an unprivileged user and only the code that needs additional powers runs as root using a tool called "rootwrap".

This talk discusses the evolution that led to the current rootwrap design, why it has proven to be completely inadequate in practice, and presents a new "privsep" alternative currently being worked on within Oslo.