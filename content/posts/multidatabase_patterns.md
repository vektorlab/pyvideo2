---
Category: 'DjangoCon 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/djangocon-2010/38_multi-database-patterns.flv
ThumbnailUrl: 'http://a.images.blip.tv/Robertlofthouse-MultidatabasePatterns241.png'
speakers: [Malcolm Tredinnick]
tags: [database, djangocon, djangocon2010, multipledatabases]
---
Multi-database patterns

Presented by Malcolm Tredinnick

A tour through four common "multiple database" usage patterns and how they can
be implemented and utilised with Django. We'll talk about the strengths and
weaknesses of each pattern and why you might not need any of them.

Abstract

There are a few good reasons a system might want to interact regularly with
multiple databases. “Because it’s what cool people do” is not one of those
reasons. Most multi-database usages fall into one of four main classes:

  * Separation by function. All data of one type in one database, all data of another type in some other database. 
  * Separation by sharding. Data of a particular type (e.g. user records) is split across multiple databases, each database holding a shard of the whole data. 
  * Data replication (separation by access). Some pieces of data are synchronized to multiple machines. Writes might go into one or more masters and reads normally come from the slaves. 
  * Data augmentation/shadowing. Data in one database is added to or entirely replaced by data from another database. Can happen during development when reading from a production snapshot whilst trying out changes to some tables or data only against a local database. 

Obviously, combinations of these classes are possible, such as replicated
sharded data in a huge site. There are tricks and traps to the way a developer
talks to each of these sorts of setups. I'll spend a few minutes showing
credible examples of the usage of each as well as when you might be over-
engineering by going that way. All four access patterns are possible in Django
1.2, with varying degrees of ease of use and I'll show the type of code
required in each case.

