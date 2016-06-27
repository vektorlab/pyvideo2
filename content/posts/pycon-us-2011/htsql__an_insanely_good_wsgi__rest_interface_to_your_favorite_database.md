---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/365_htsql-an-insanely-good-wsgi-rest-interface-to-your-favorite-database.mp4
Speakers: [Clark C. Evans]
Tags: [htsql, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011HTSQLAnInsanelyGoodWSGIRESTInterfaceToYour159.png'
Title: 'HTSQL - an insanely good WSGI / REST interface to your favorite database'
date: '2011-03-11'
---
The HTSQL processor is a high-level URI-based query language for relational
databases such as SQLite, PostgreSQL or MySQL. Since it's written in Python,
it is easy to integrate and generates immediate value as the core of your
application's custom reporting engine. HTSQL is like the Django or SQLAlchemy
ORMs in that it generates SQL, but unlike an ORM in that its design center is
completely different -- it was created for hard core reporting and not object
to relational mapping. Hence, it is a wonderful complement to existing WSGI-
based applications to easily create dashboards, complex reports. We use HTSQL
as a REST reporting interface for data integration and ad-hoc queries.

This talk will have two parts. In the first part we'll give a brief overview
of the rationale and design of the query language. In the second part, we'll
show how to hook the HTSQL processor into your WSGI application and how to
make custom commands, such as a simple calendar output from a table containing
a date column.

The talk will be presented by Clark Evans, HTSQL was developed by Kyrylo
Simonov. The main HTSQL site is [http://htsql.org](http://htsql.org) and the
code is at [http://bitbucket.org/prometheus/htsql](http://bitbucket.org/promet
heus/htsql). It'll be similar to previous talks, such as
[http://htsql.org/talks/20101103.html](http://htsql.org/talks/20101103.html).
