---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=PJ5vUz9FJcw'
Speakers: [Hynek Schlawack]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/PJ5vUz9FJcw/hqdefault.jpg'
Title: 'The Sorry State of SSL'
date: '2014-07-22'
---
The rule of thumb for people without degrees in cryptography on securing data on the Internet is “GPG for data at rest. TLS for data in motion”. And it’s actually a very good rule everyone should follow.

The only kicker though is that configuring (and using!) TLS properly is not as simple as it sounds and if you’re not diligent as a user, developer, and ops engineer, you can easily compromise your data’s security despite best effort of everyone else.

This talk will be multifaceted; you will learn:

- how SSL and TLS roughly work and why their state is sorry,
- server- and client-side duties for best possible security,
- what alternatives you have for using TLS in Python,
- things to keep in mind when configuring servers,
- and what perils outside your control still can trip you up.

In other words, the leitmotif is to show you the most common traps you should know about when using and deploying applications relying on TLS for transport layer security and how to avoid them. 