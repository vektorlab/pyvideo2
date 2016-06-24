---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=lNh-tS8i-J4'
Speakers: [Alex Hill]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/lNh-tS8i-J4/hqdefault.jpg'
Title: 'Many-to-many, minus the middleman'
date: '2015-08-04'
---
This talk is about an alternative Django ManyToManyField implementation that uses (abuses?) PostgreSQL's full-text search engine instead of an intermediary table to store its relationships. As well as showing off some handy things you can do with this field, we'll talk along the way about full-text search in Postgres, inverted indexes, and how Django's ManyToManyField is implemented.

Behind the scenes, ManyToManyField uses an intermediary table to record its relationships – a classic relational database technique you most likely mastered in Databases 101. But to believe some present-day commentators, classic relational databases with their fixed schemas and their ACID habit belong back in the 70s where they came from.

Enter Postgres, the hip, switched-on parent who works as a public defender and gets on uncomfortably well with your friends. Postgres builds on a wealth of relational history while embracing modern non-relational ideas in a thoughtful, sane way.

In this talk, we'll press full-text search, one of Postgres' repertoire of many useful features, into a service it performs remarkably well despite being designed for quite a different purpose. Code and benchmarks provided!

