---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=bgV39DlmZ2U"'
Speakers: [Malcolm Tredinnick]
Tags: [django, django-orm]
ThumbnailUrl: 'http://i.ytimg.com/vi/bgV39DlmZ2U/hqdefault.jpg'
Title: '"The Dungeon Master''s guide to Django''s ORM"'
date: '2012-09-05'
---
Django's database layer is a necessarily complicated piece of code. It is a
very powerful API that works more or less seamlessly across multiple database
storage systems, smoothing over many of the inconsistencies and implementation
differences that go with the territory. This is great for developers who use
Django.

It's a little less awesome for the maintainers of that code; working in that
environment is fairly difficult. Still, we all like a challenge. Problem is:
where to start? Coming to grips with the ORM code isn't easy. The code is well
written and documented, but the entry points are particularly well highlighted
and, really, the sheer mass of code is an obstacle to be overcome.

This talk will look at the various layers of the ORM, from the public
gateways, to the semi-public doors into the implementation, to the deeper
internals and down to the interaction with databases. In effect, following the
journey of a couple of adventurous young queries as they traverse the pathways
to bring back some data, smelted into just the right format.

The goal is to provide some kind of mental map of the code. Some tips for
orienting yourself in the future and how to examine new nooks and corners
without losing your mind. We obviously cannot cover everything, but let's go
over the common paths and show how the other pieces hang off that backbone.

Along the way, we'll put some of the details into historical perspective.
Getting inside the mind of previous adventurers might help understand why
things are the way they are.

