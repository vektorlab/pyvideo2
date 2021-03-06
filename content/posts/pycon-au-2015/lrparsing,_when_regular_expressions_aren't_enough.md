---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=9PQsCmOeYwU'
Speakers: [Clinton Roy]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/9PQsCmOeYwU/hqdefault.jpg'
Title: 'Lrparsing, when regular expressions aren''t enough'
date: '2015-08-04'
---
Lrparsing is a fast, well documented and tested parsing infrastructure for Python. Parsing infrastructures are used when the input to be parsed is too complex to be done by regular expressions alone. Parsing infrastructures are ideally suited to parsing programming languages and configuration files. Lrparsing is roughly equivalent to the combination of Flex and Bison, except completely implemented in Python, and is thus very Pythonic.

The rest of the abstract uses the following Python snippet as an example:

1 if option else 2

lrparsing provides both a lexer (which breaks the input down into tokens, e.g.:

 ['1', 'if' , 'option',  'else', '2']

and a parser generator, which produces a concrete parse tree:

(«ternary», («bool», 'option'), («expr», '1')), («expr», '2')))

 Lrparsing provides Pythonic syntax support to easily construct parsers for programming languages, Domain Specific Languages and configuration file formats.

Lrparsing is very well suited to constructing Concrete Parse Trees but has little support for creating Abstract Syntax Trees (AST), which are much easier to use: My work has added Abstract Syntax Tree support to lrparsing, yielding exactly the same AST nodes that the Python AST module supports:

IfExp(condition, 1, 2)

This talk will give an overview of the major features of Lrparsing, then look at my work to add AST support. 
