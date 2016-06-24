---
Category: 'PyCon US 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2010/265_ply-and-pyparsing-93.m4v
Speakers: [Andrew Dalke]
Tags: [ply, pycon, pycon2010, pyparsing]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2010PLYAndPyParsing93735-488.jpg'
Title: 'PLY and PyParsing (#93)'
date: '2010-02-19'
---
PLY and PyParsing

  
Presented by Andrew Dalke

  
Got a text parsing problem? In most cases using string manipulation and
regular expressions will solve it for you. But when the input is complex, try
reaching for a parsing system to help out.

  
The two most popular in Python are PLY and PyParsing. PLY follows the lex/yacc
tradition with a domain specific language to describe the tokens and grammar.
It was built with both error diagnostics and performance in mind. PyParsing is
a recursive descent parser which expresses the format as a Python data
structure. It make no distinction between lexer and grammar and has a uniform
callback system which makes certain types of data extraction very easy.

  
In my talk I'll show the basics of how to use both systems for several
different format parsing tasks, of different complexity. This will let you see
how to use the parsers and understand more of the tradeoffs between
complexity, readability, error handling, and performance.

