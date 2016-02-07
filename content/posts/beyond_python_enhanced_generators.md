---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=yWR00Y6tkC8'
Speakers: [Erik Groeneveld]
Tags: [generators, search]
ThumbnailUrl: 'http://i.ytimg.com/vi/yWR00Y6tkC8/hqdefault.jpg'
Title: 'Beyond Python Enhanced Generators'
date: '2011-07-24'
---
Right after the introduction of PEP342 (Enhanced Generators) we started to
decompose programs into generators. It was soon discovered that for real-life
problems one would need something like "yield from", as is described in
PEP380. At that time, we already had a similar solution called
'[compose](http://weightless.io/compose)', which we adapted to PEP380.

After 5 years working with 'compose', we found a small set of other features
that are essential if you want to use Enhanced Generators not only as a way of
lightweight command scheduling, but also a a pipe-line, or parser. Indeed, the
latter concepts are what real co-routines are about.

This talk introduces what is needed on top of PEPs 342 and 380 based on
experience with decomposing big enterprise search engines into co-routines.
Parts of it have been presented on SPA (2008) and EuroPython (2010).
Understanding of Enhanced Generators is a prerequisite.

Experience has shown that the topic is subtle enough to require quite some
time for full understanding, hence the suggestion for a 90 min slot.

