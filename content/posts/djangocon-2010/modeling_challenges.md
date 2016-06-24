---
Category: 'DjangoCon 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/djangocon-2010/42_modeling-challenges.flv
Speakers: [Malcolm Tredinnick]
Tags: [djangocon, djangocon2010, model]
ThumbnailUrl: 'http://a.images.blip.tv/Robertlofthouse-ModelingChallenges314.png'
Title: 'Modeling challenges'
---
Modeling Challenges

Presented by Malcolm Tredinnick

How would you model players, umpires and coaches in baseball data when the
same person can switch roles over the course of their life? How about servers
in racks with power boards attached (and cords running across the room to
remote boards)? Come along to see one approach to create minimal and well-
performing models for such real-life situations.

Abstract

The slightly over-simplified but useful rule of thumb when creating database
schema is “normalize until it hurts, [then] denormalize until it works.” If
only people didn’t skip the first step so often. Using a data modeling layer,
such as Django's models, doesn't absolve the system architects from the need
to create good design. It also doesn't require them to do so, since you can
get away with a lot of sub-optimality with many data sets.

The real difficulty here, though, is that the trade-off between text-book
ideal modeling and easy to use is difficult to judge and takes practice to
develop.

This talk will walk some interesting cases of model design that I've
encountered recently. I'll explain how I approached the problem and what we
ended up with. These will include:

  * Modeling people who might simultaneously play different roles in the system. For example, a person who was a baseball player and then became a coach — each role has different attributes attached to it. 
  * Modeling what appears to be a triangular dependency relationship with minimal redundancy in the data description and without needing really long query filters to access things. 
  * Handling date ranges (or other measured data) of different degrees of accuracy and precision. 

This won't be a talk on theoretical database design. Rather, concrete examples
of creating such designs and guiding the decisions by what might work best in
the final Django code. Hopefully, by listening to one person's approach
(mine!), people faced with similar challenges will have another possible
attack method in their toolbox.

