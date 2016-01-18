---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=xjikvIHjvHs"'
ThumbnailUrl: 'http://i.ytimg.com/vi/xjikvIHjvHs/hqdefault.jpg'
date: '2014-07-24'
speakers: [Alexey Malashkevich]
tags: []
---
[Pony ORM](http://ponyorm.com) is an object-relational mapper implemented in Python. It allows writing advanced queries to a database using plain Python in the form of a generator expression. This way queries look very concise.

The main feature of Pony is to provide a method to write declarative queries to databases in pure Python using generators. For this purpose Pony analyzes the abstract syntax tree of a generator and translates it to its SQL equivalent.

Following is a sample of a query in Pony:

    select(p for p in Product if "iPad" in p.name and p.price >= 500)

This query translates to SQL using a specific database dialect. Currently Pony works with SQLite, MySQL, PostgreSQL and Oracle databases.

In this talk one of Pony ORM authors will go through the process of the query translation and dig into the implementation details.

Attendees are going to walk away with the understanding of: 

1. Principles of building a programming language translator
2. Python to SQL translator implementation details 
3. Approaches for creating a pluggable translator architecture 

The presentation outline:

- Why Python generators are good for representing SQL queries
- Main stages of Python to SQL translation overview
- Decompiling Python bytecode into Python AST
- Translating Python AST to database-independent SQL representation
- Generating SQL for specific database
- Pluggable translator architecture
- Performance concerns: is such way of building SQL slower or faster then Django's and SQLAlchemy's?