---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=hAqtC_c2x1s"'
ThumbnailUrl: 'http://i.ytimg.com/vi/hAqtC_c2x1s/hqdefault.jpg'
date: '2011-07-07'
speakers: [Andrew Godwin]
tags: [ep.io, hosting, infrastructure, postgresql, redis, scalable, web]
---
At ep.io we built a Python hosting platform from the ground up, designed to
run large numbers of web applications on a small number of physical machines
both securely and in a reasonably scalable way. This talk will show you how we
built our infrastructure - using Redis, eventlet, PostgreSQL and more - and
what lessons we learnt from our first few thousand deploys.

See how we split services into multiple processes and greenthreads; the pains
of building a cooperatively-multitasking PTY module; how Redis isn't the
answer to everything, but is still very useful; how to persuade third-party
software to work securely in a shared environment; and how important it is to
have good logging, especially when you have more than five servers.

