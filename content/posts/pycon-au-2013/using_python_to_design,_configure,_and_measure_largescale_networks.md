---
Category: 'PyCon AU 2013'
Copyright: 'CC-BY-SA'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=EGK5jjyUBCQ'
Speakers: [Simon Knight]
Tags: []
ThumbnailUrl: 'http://i1.ytimg.com/vi/EGK5jjyUBCQ/hqdefault.jpg'
Title: 'Using Python to design, configure, and measure large-scale networks'
date: '2013-07-06'
---
AutoNetkit is an open-source project to automatically build network configuration files for routers including Quagga, Cisco and Juniper, with complicated protocol configurations, all from a simple input graph --- which could even be drawn in a program such as yEd. 

AutoNetkit was started at the University of Adelaide, and developed further at Cisco, with collaborators from both research and industry.
It is being used at major router vendors, by network operators, and in university teaching, and in research publications including experiments with over 800 virtual routers --- nearly impossible to configure by hand.


This is all powered by Python, and we make significant use of the excellent packages available.

This talk will present a brief overview of what the AutoNetkit project is about and why we chose Python.

I will give an over view of our data model, and how methods such as __lt__ __eq__ __contains__ __getattr__ __setattr__ and __iter__ allow elegant yet expressive network design, such as using list comprehensions.

I will cover how we use the various modules, including:
- NetworkX graphs
- Netaddr IP addressing
- Mako Templates
- Exscript for scripting deployment
- TextFSM parsing of measurement
- Tornado to serve a browser-based d3.js visualisation framework
- Using IPython notebooks for interactive tutorials

We've spent quite a bit of time with Python on this project. This talk will pass on the our favourite Python language features and package we've found along the way.
It will be both a case study in using Python for a large-scale project, and an overview of useful packages.