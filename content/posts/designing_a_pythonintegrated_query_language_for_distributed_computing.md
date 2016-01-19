---
Category: 'PyCon APAC 2014'
Copyright: 'youtube'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=wxlq0HkE3zw"'
Speakers: [Jiwon Seo]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/wxlq0HkE3zw/hqdefault.jpg'
Title: '"Designing a Python-integrated query language for distributed computing"'
date: '2014-06-27'
---
Python becomes increasingly popular in the domain of big data analysis. Many big data frameworks such as Hadoop now support Python to some extent. PySociaLite is a new big data framework developed at Stanford. It is designed from beginning to be fully integrated into Python. In PySociaLite, SQL-like queries (called SociaLite) are directly embedded within Python code; the queries can access Python variables and functions, so there is full inter-operation between SociaLite and Python.

In this talk, I will give a brief overview of SociaLite, then mainly present the techniques for the integration of SociaLite into Python. SociaLite builds on top of well-known programming concepts -- tables and relational operations -- and it allows users to declare distributed tables to perform, for example, distributed join operations. For the integration of SociaLite into Python, we basically extend Jython interpreter to process embedded SociaLite queries. More specificaly, we use PyParsing to recognize SociaLite queries and re-write the queries into Java function calls. We also use lesser-known Python features, such as import hooks to process SociaLite queries within imported modules. To access Python functions within SociaLite, Jython interpreter instance (from which SociaLite queries are executed) is passed to SociaLite runtime system, and used to lookup and access Python functions. For the distributed execution, Python functions are serialized (as well as its PyCode object) and copied to cluster machines. 

Time permitting, I will give a demo of PySociaLite; SociaLite queries will be executed interactively within (extended) Jython shell and demonstrate the inter-operation between SociaLite and Python.


About the speaker

Jiwon Seo is a PhD student in Stanford university, studying parallel query language for data analysis. He contributed to Python in various ways; for example, he implemented PEP 289 (Generator Expressions) and PEP 3102 (Keyword-Only Arguments).

He designed and implemented a parallel and distributed query language, called SociaLite. The SociaLite compiler generates efficient parallel/distributed code from user queries. SociaLite queries can be embedded in Python programs, allowing users to enjoy flexibility of Python and efficiency of SociaLite. More information is in <http://socialite-lang.github.io/>