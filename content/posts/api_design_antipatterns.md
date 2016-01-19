---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/445_api-design-anti-patterns.mp4
Speakers: [Alex Martelli]
Tags: [api, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011APIDesignAntipatterns897.png'
Title: '"API Design anti-patterns"'
date: '2011-03-11'
---
API Design Anti-Patterns

Presented by Alex Martelli

Designing interfaces so that other code can interact with ours (whether our
code is a library, framework, application, website...) is a very common and
clearly crucial activity, but fraught with dangers -- stuff we all keep doing
wrong time after time. This talks shows some common cases of API design errors
encountered in the wild, with tips on how to avoid them when you design your
next API.

Abstract

Whenever we write code we should always be thinking about how other code
(whether our own, or other people's) will interact with ours (an "API", in
common parlance). Indeed, the most common and terrible mistake in API design
is... not doing any! -- i.e., not providing any designed, architected way for
other code to interact with ours. That's fortunately less common when "our
code" is a library or framework;-), but, alas!, sadly widespread when "our
code" is an application or website -- that's why questions about screen-
scraping the web and simulating keystrokes and mouse gestures need be so
tragically frequent all over the web.

Once past the obvious hurdle of not having any API at all, there's still
plenty of ways we can go badly wrong in the process of designing one -- and
many of those ways fall into recognizable categories, i.e., patterns.
Specifically, since they're frequently observed categories of defective
design, they're anti-patterns -- and that's what this talk is in fact about
(as the smartest among you could tell from the title...).

I'm eminently qualified to present on this subject, since, in a lifetime spent
mostly stumbling into software (after actually qualifying to design hardware
in college, but only doing that for a few years), I've been responsible for
more of my shares of API design fumbles (plus, of course, just like every
other programmer, I've done my share of swearing at the design fumbles of
other API designers). And, as novelist Richard Bach reminds us, "You teach
best what you most need to learn"!-)

