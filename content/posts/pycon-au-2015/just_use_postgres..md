---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=UgcC_bY4rPg'
Speakers: [Rhys Elsmore]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/UgcC_bY4rPg/hqdefault.jpg'
Title: 'Just Use Postgres.'
date: '2015-08-04'
---
Making use of the latest database for your data is considered trendy and edgy, with vendors promising unrealistic expectations when it comes to capabilities of these systems. Furthermore, communities such as Hacker News enforce the idea that you must use the latest and coolest technology in order to be a ‘rockstar’ engineer.

Marketing buzzwords like ‘real-time’, ‘distributed’, ‘high-availability’, and ‘schemaless’ impact our design decisions, and the expectation for applications to be ‘scalable’ often forces developers to prematurely introduce complexity and anti-patterns into their applications by making use of these untested and immature data stores.

Forget about adding the latest trendy data store into your stack; just use Postgres.

This talk will explore the capabilities of Postgres 9.4, and various use-cases where you can involve it as your primary datastore. I will cover some of the projects at Heroku where we have used Postgres, such as:

- Quickly querying over 300M records to get a list of all users on a particular server at a particular point in time.
- Providing almost real-time aggregations of all Heroku customer’s usage.
- Joining 3 different tables on 3 different database servers without any external code.
- Creating a ‘social graph’ of all of Heroku’s users based on commonly used IP addresses.
- Ensuring that coupon codes are used only once, preventing attackers from exploiting ‘race condition’ bugs.

 In particular, I will focus on topics such as:

- Storing, indexing, and querying schemaless data.
- Materialized Views.
- NOTIFY/LISTEN.
- Storing and querying time-series data.
- Updatable views.
- Foreign tables.
- Recursive views.
- Stored functions.
- Range Types
- Partitioning and Sharding data.

Each topic will include links to sample schemas and iPython notebooks so you can take these examples home with you.
