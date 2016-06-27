---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=4XRrLdogkdA'
Speakers: [Anders Hammarquist]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/4XRrLdogkdA/hqdefault.jpg'
Title: 'Multi-document consistency with MongoDB'
date: '2012-07-05'
---
When working with MongoDB, especially if you are coming from (or converting an
application) the SQL world, you will probably miss the SQL transaction, which
gives you, among other things, atomic writes. MongoDB only provides atomic
writes to one document. We will show you how you can implement multi-document
writes that are, if all writers cooperate, consistent across multiple
documents and either writes all changes completely or fail without writing any
changes. Audience: People who are looking at SQL alternatives, but still need
some sort of transaction-like consistency. Understanding of parallellism
issues, race conditions and deadlocks, may be helpful. MongoDB knowledge is
not needed. Slides online at:
[http://www2.openend.se/~iko/ep2012/](http://www2.openend.se/~iko/ep2012/)
