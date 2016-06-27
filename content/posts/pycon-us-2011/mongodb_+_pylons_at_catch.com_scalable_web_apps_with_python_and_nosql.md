---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/399_mongodb-pylons-at-catch-com-scalable-web-apps-with-python-and-nosql.mp4
Speakers: [Niall O'Higgins]
Tags: [casestudy, mongodb, nosql, pycon, pycon2011, pylons, scalable]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011MongoDBPylonsAtCatchcomScalableWebAppsWithPy842-535.jpg'
Title: 'MongoDB + Pylons at Catch.com: Scalable Web Apps with Python and NoSQL'
date: '2011-03-11'
---
MongoDB + Pylons at Catch.com: Scalable Web Apps with Python and NoSQL

Presented by Niall O'Higgins

The Catch.com backend provides an API for publishing and querying your
personal data - used by many hugely popular Android, iOS and Web clients. We
ported this system to Python and MongoDB, using the Pylons Web framework. This
talk details our reasoning for choosing - and experiences with - these
cutting-edge Web and NoSQL database technologies in a high-traffic, real-world
production system.

Abstract

Faced with the limits of our initial Catch.com Java/BDB backend implemention,
we evaluated various alternative technologies including Amazon SimpleDB,
MySQL, Cassandra and MongoDB. Eventually we settled on Python, Pylons and
MongoDB.

We found Python and MongoDB gave us unique flexibility with our data model,
allowed us to scale for increased reliability and performance and decreased
feature development time - and in this talk we'll describe exactly how.

While there are many advantages, Python/Pylons and MongoDB (as a relative
newcomer on the database scene) certainly have issues and limitations which
must be taken into careful consideration for any real-world production
deployment.

We compare MongoDB with other database technologies such as more traditional
RDBMS like MySQL and competing NoSQL options such as Cassandra, CouchDB and
BDB.

We give a detailed introducton to data modeling in MongoDB - with special
attention paid to how this differs from a traditional relational system - the
operators provided by its rich query language and utilizing advanced features
such as GeoSpatial indexing, Replica Sets, Sharding - and how to deal with
some of the more publicized limitations of the system (such as single-server
durability).

While much of this talk will be about using MongoDB with Python, we will also
touch on issues surrounding production deployment of the Pylons Web framework,
including how we work around the GIL to take advantage of multi-core machines.
