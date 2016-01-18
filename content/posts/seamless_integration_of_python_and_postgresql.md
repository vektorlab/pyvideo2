---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=99AoONzl-Ik"'
ThumbnailUrl: 'http://i.ytimg.com/vi/99AoONzl-Ik/hqdefault.jpg'
date: '2012-07-05'
speakers: [H Krossing]
tags: []
---
Presenting a better way of using PostgreSQL from python with Simple to use way
to avoid moving data back and forth to client for just for processing while
still maintaining your code in client code and getting all the benefits of
server-side programming with ease of Python. access to data without writing
SQL for simple usage while SQL is still available where appropriate, like
complex data analysis This is achieved by the following: decorators which ship
python code to be executed in database, with potentially 100x speedup for some
use cases direct building of query plans bypassing SQL generation and parsing
Some more infrastructure is presented which is needed for using code-shipping
in more complex scenarios like django extra import hooks in server for loading
python modules from caller (client) extra import hooks for importing modules
from database loadatstartup modules for pl/python ways to scale this type of
application by sharding (a.k.a. horisontally scaling) it using pl/proxy

