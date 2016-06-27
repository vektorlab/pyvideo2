---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/389_reverse-engineering-ian-bicking-s-brain-inside-pip-and-virtualenv.mp4
Speakers: [Carl Meyer]
Tags: [pip, pycon, pycon2011, virtualenv]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011ReverseengineeringIanBickingsBrainInsidePipAnd764.png'
Title: 'Reverse-engineering Ian Bicking''s brain: inside pip and virtualenv'
date: '2011-03-11'
---
Reverse-engineering Ian Bicking's brain: inside pip and virtualenv

Presented by Carl Meyer

Pip and virtualenv: many use them; not so many understand just how they work
their magic. If you're a pip/virtualenv user but haven't yet dared crack the
lid (or you have, and found it a bit difficult to follow), come along for a
fast-paced guided tour. Knowing these tools will help you make more effective
use of them, and might also turn you into a contributor.

Abstract

Pip and virtualenv are widely used in the Python world, but for the size of
their user base don't receive many code contributions, and many users have
misconceptions about how they actually work.

This talk will cover a bit of advanced use of pip and virtualenv, but mostly
we'll dive into the source code, mapping it out with a high-level view and
diving into the guts of particularly interesting bits. By the end of the talk,
you'll have a good idea exactly how pip and virtualenv do their magic, and
where to go looking in the source for particular behaviors or bug fixes. We'll
walk through the creation of a virtualenv step-by-step, and trace a typical
"pip install -r requirements.txt" and "pip uninstall" through the code paths
they follow.

I'll know the talk was a success when I see the pull requests!
