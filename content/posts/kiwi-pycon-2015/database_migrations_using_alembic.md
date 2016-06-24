---
Category: 'Kiwi PyCon 2015'
Copyright: 'CC BY-SA'
Language: 'English'
SourceUrl: 'http://youtu.be/xzsbHMHYI5c'
Speakers: [Tim Mitchell]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/xzsbHMHYI5c/hqdefault.jpg'
Title: 'Database migrations using alembic'
date: '2015-09-06'
---
Managing database schema changes can be a challenging process. From the schema change itself to keeping test (and user!) data in sync with the schema across multiple development branches can be a headache. Alembic is paracetamol for this change management headache. Alembic is a companion package to sqlalchemy for creating database schema migrations. This talk will introduce alembic, demonstrate how it is used to generate schema deltas and migrate database schemas. The talk will discuss manually adding data migration to a schema migration script and describe how using alembic has changed our development process. Some familiarity with databases and sqlalchemy will be assumed.