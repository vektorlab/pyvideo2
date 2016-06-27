---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=bPJKYrZjq10'
Speakers: [Alex Martelli]
Tags: [architecture, design, patterns]
ThumbnailUrl: 'http://i.ytimg.com/vi/bPJKYrZjq10/hqdefault.jpg'
Title: 'Python Design Patterns'
date: '2011-07-13'
---
A completely misguided meme has long been going around: that Python doesn't
have, or need, any Design Patterns. This terrible meme may spring from not
realizing what the Gang Of Four state so plainly in their historical "Design
Patterns" book: which design patterns are useful DOES depend on the
programming language one targets - design is NOT independent of
implementation, as the epic-fail "Waterfall" Methodology Pattern would
suggest. What patterns apply to a design, depends to some extent on what
implementation technologies will be used to realize that design.

If you focus on some "classic DPs" that are basically workarounds for some
other language's lack of garbage collection, or for a clumsy static-typing
system, those may indeed be worthless for Python. But many other DPs are
perfectly useful and applicable, and Python's strengths as a language afford
riffing on them to develop highly Pythonic, powerful, productive variants.

In this talk, I analyze some of my favorite pattern families - e.g., Template
Method and its variants, Dependency Injection and its ilk, Callback and
friends - in a highly Pythonic context. Non-pattern Idioms, and Patterns that
aren't really Design Patterns but rather Architecture or Methodology ones,
make cameo appearances.

Goals: remove from your system any residue of the pernicious meme about Python
not having or needing design patterns. Prereqs: experience designing and
developing software; intermediate-level Python knowledge.
