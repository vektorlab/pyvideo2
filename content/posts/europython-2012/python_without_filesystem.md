---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=xWY0UQn3dcA'
Speakers: [Arnaud Fontaine]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/xWY0UQn3dcA/hqdefault.jpg'
Title: 'Python without filesystem'
date: '2012-07-04'
---
Recent cloud architecture are heavily based on key-value storage databases
rather than distributed filesystems. While the data itself is usually stored
in scalable database, the source code is mainly kept on the filesystem.
However, having the source code on filesystem raises a lot of issues for cloud
applications and more generally for transactional web applications supposed to
be deployed on a large number of servers: Everytime the source code is
modified, it has to be synchronized on all the nodes somehow and the
application server must be restarted, therefore implying downtime or
inconsistency. Usually, the developer cannot directly modify the source code
as this task is left to the administrator. This talk will show how source
code, including modules and their classes, can be migrated away from
filesystem, thanks to import hooks, meta classes, reflection and
metaprogramming provided by Python, and the different challenges involved:
Technical: modules and classes must be loaded and reset while carefully
considering concurrency and database issues and ensuring that the system will
stay usable whatever happens and without breaking existing class instances.
Also, developers must be efficient with the new system, including convenient
source code edition and meaningful backtraces. Performance: having dynamic
modules and classes involved a performance tradeoff which should be kept to
the minimum. Security: as the source code is dynamically loaded from the
database, extra care must be taken care of compared to filesystem source code
where the source code is never supposed to change once the applications has
been started. In order to give practical examples of how this migration can be
achieved, two examples will be studied and explain thoroughly, based on the
experience I have acquired through the implementation for ERP5 I have worked
on during the past year: First, through a basic WSGI application based on a
lightweight web application framework to explain the basics behind having
Python source code available in a transactional key-value storage database and
more precisely how modules and their classes can be dynamically loaded and
reset on-demand upon modifications while keeping good performances. This
usually involved specific features from the database point of view which will
also be discussed. Secondly, through ERP5 which is mainly known as an open
source ERP based on Zope and thus ZODB, and as such it provides features an
ERP typically provides, but it is also used for a wide range of other
purposes. Therefore, this will give a more real-world example on how this
migration has been performed on a complex web application where 90% of the
code is going to be moved away from filesystem into the ZODB.