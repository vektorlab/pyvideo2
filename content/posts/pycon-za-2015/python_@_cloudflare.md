---
Category: 'PyCon ZA 2015'
Copyright: ''
Language: 'English'
SourceUrl: 'http://youtu.be/lrLV93EFO0g'
Speakers: [Gideon Redelinghuys]
Tags: [room 215]
ThumbnailUrl: 'https://i.ytimg.com/vi/lrLV93EFO0g/hqdefault.jpg'
Title: 'Python @ CloudFlare'
date: '2015-10-01'
---
CloudFlare protects and accelerates any website online. Whether it's protecting large customers from 160Gbps DDOS attacks, dealing with normal Reddit traffic, Universal SSL or providing one of the fastest DNS servers in the world we need to stay up, work fast and deploy fast.

To this end we have two large Python projects we use at CloudFlare. One is the popular configuration manager Salt. We provide patches, features and bug reports on regular intervals to the Salt project. The other is an internal tool called CFSetup. CFSetup allows us to do the following with a few simple commands: spin up Docker containers that reflect machines in production, spin up a tightly coupled stack of Docker containers that reflect our software and hardware stacks, run build environments inside of well defined Docker containers to ensure that the compiled end-product was built using the same libraries that are on the production machines, and various other utility features.

This talk will cover how Salt works, how we've extended it to scale up and how we've had to debug it. It also cover how we've managed to build a layer on top of Docker to make it easier to use for ad-hoc testing and developing and what it's like interacting with Docker using Python.
