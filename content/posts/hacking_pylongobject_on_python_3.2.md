---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=9tzd45ho8gE"'
ThumbnailUrl: 'http://i.ytimg.com/vi/9tzd45ho8gE/hqdefault.jpg'
date: '2011-07-13'
speakers: [Cesare Di Mauro]
tags: [hacking]
---
Beginning with Python 3 the old integer ("int") type has gone leaving the
place to "long", which replaced it giving a unique, uniform type to deal with
integers. However longs need a more complex structure which effectively
dropped a bit of Python 3.x performance. Looking at their implementation, an
idea grown that can help to improve the situation on common sceneries (using
"short" integers). A slightly changed structure will be presented and compared
with the old PyIntObject and the current Python 3.2 PyLongObject, along with
some optimizations, thoughts, and issues found on the road, which will show
the effort required by such change on a Python core element.

