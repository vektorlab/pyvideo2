---
Category: 'PyCon ZA 2015'
Copyright: ''
Language: 'English'
SourceUrl: 'http://youtu.be/lXhypJUbxVM'
Speakers: [Azhar Desai]
Tags: [Room 215]
ThumbnailUrl: 'https://i.ytimg.com/vi/lXhypJUbxVM/hqdefault.jpg'
Title: 'OpenCanary: a new Python-based honeypot'
date: '2015-10-01'
---
Honeypots: a great idea tempered by over a decade of glorious misapplication resulting in a slow relegation to the realm of academia and slightly dubious research. But it doesn’t have to be that way. In August 2015 we released OpenCanary, the Open Source version of our commercial Python-based honeypot. 

Traditional honeypots aim to reveal attacker tools, techniques and procedures, by entrapping attackers through emulation (or instrumentation) of common protocols and services. They are typically installed standalone, and seldom updated. We argue that this honeypot approach is outdated; current organisations struggle far more with <em>identifying breaches</em> than identifying the version of some generic rootkit installed post-breach. 

OpenCanary changes that, treating the honeypot as an internal distributed sensor rather than a standalone alert generator. Each event reported is a high-quality indicator of investigation-worthy activity, and each OpenCanary instance feeds event data to a correlator which produces single alerts even in the face of network-wide scans. With such a high signal-to-noise ratio, every alert requires investigation. This is in contrast to the stream of alerts produced by tools such as anti-virus, network IDS or traditional honeypots.

OpenCanary wound up relying on Python for the majority of the code. The Python eco-system provided support that sped up development and, more importantly, deployment. However it didn’t take us the full distance.

In this talk, we provide a brief background on honeypots, discuss the design of OpenCanary, delve into the challenges experienced and our plans for the project. Along the way, we’ll demo the trivially installable OpenCanary, configure a few fake services and provide an outsider’s view of developing in Python.