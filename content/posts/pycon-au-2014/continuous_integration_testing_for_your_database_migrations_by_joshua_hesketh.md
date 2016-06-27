---
Category: 'PyCon AU 2014'
Copyright: 'http://www.youtube.com/t/terms'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=z_q5BaniZH0'
Speakers: [Joshua Hesketh]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/z_q5BaniZH0/hqdefault.jpg'
Title: 'Continuous Integration Testing for Your Database Migrations by Joshua Hesketh'
date: '2014-08-11'
---
This is a talk about how OpenStack does database migration continuous integration, and how other projects might be able to learn from what we've done.

OpenStack is an interesting project in that it runs in a variety of different scale scenarios. There are very small deployments of only a few machines, and large public clouds with thousands of machines. The OpenStack project takes Continuous Integration (CI) very seriously, and runs a suite of unit and integration tests on all proposed patches.

One thing we weren't very good at testing though, was database upgrades. We have unit tests for many of them, but we don't know how these upgrades affect real users in the field. As a response, we worked on adding database migration testing to our CI environment. This new test infrastructure is open source (https://github.com/stackforge/turbo-hipster), and extensible. It currently runs tests on smaller databases, as well as a largish real user database. It has already caught two significant performance problems in database migrations.

This talk will cover how we built the test infrastructure (in python!). It will cover what we've learned from the 12 months of running it - time that we'll have had by the conference day. It will tell a story about some of the bugs we've found and how we fixed them.
..
