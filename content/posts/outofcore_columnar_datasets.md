---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=-lKV4zC1gss"'
Speakers: [Francesc Alted]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/-lKV4zC1gss/hqdefault.jpg'
Title: '"Out-of-Core Columnar Datasets"'
date: '2014-07-25'
---
It is a fact: we just entered in the Big Data era.  More sensors, more
computers, and being more evenly distributed throughout space and time
than ever, are forcing data analyists to navigate through oceans of
data before getting insights on what this data means.

Tables are a very handy and spreadly used data structure to store
datasets so as to perform data analysis (filters, groupings, sortings,
alignments...).  However, the actual table implementation, and
especially, whether data in tables is stored row-wise or column-wise,
whether the data is chunked or sequential, whether data is compressed or not,
among other factors, can make a lot of difference depending on the
analytic operations to be done.

My talk will provide an overview of different libraries/systems in the
Python ecosystem that are designed to cope with tabular data, and how
the different implementations perform for different operations.  The
libraries or systems discussed are designed to operate either with
on-disk data ([PyTables] [1], [relational databases] [2], [BLZ] [3],
[Blaze] [4]...) as well as in-memory data containers ([NumPy] [5],
[DyND] [6], [Pandas] [7], [BLZ] [3], [Blaze] [4]...).

A special emphasis will be put in the on-disk (also called
out-of-core) databases, which are the most commonly used ones for
handling extremely large tables.

The hope is that, after this lecture, the audience will get a better
insight and a more informed opinion on the different solutions for
handling tabular data in the Python world, and most especially, which
ones adapts better to their needs.

[1]: http://www.pytables.org
[2]: http://en.wikipedia.org/wiki/Relational_database
[3]: http://blz.pydata.org
[4]: http://blaze.pydata.org
[5]: http://www.numpy.org/
[6]: https://github.com/ContinuumIO/dynd-python
[7]: http://pandas.pydata.org/
