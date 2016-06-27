---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/419_what-would-you-do-with-an-ast.mp4
Speakers: [Matthew J Desmarais]
Tags: [ast, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011WhatWouldYouDoWithAnAst198.png'
Title: 'What would you do with an ast?'
date: '2011-03-11'
---
What would you do with an ast?

Presented by Matthew J Desmarais

The ast module in the Python (>= 2.6) standard library provides a
representation of python code in a python data structure. We'll begin with a
discussion about what an abstract syntax tree is and why it's useful. We can
then talk about what's available in the ast module, how it works, and how you
can use it. This will be a practical session built around examples examining
and modifying live ASTs.

Abstract

I would prefer to make this a 45 minute talk with examination of code samples.

Python 2.6 introduced a new module in the standard library, ast. The first
line of the ast documentation is, "The ast module helps Python applications to
process trees of the Python abstract syntax grammar." What this means is not
obvious and many, if not most, python programmers won't know what this means.
I will begin by talking about the idea of syntax tree and how it fits into the
python execution lifecycle. I will also talk about the contents of the ast
module. I will cover the available ast.Node subclasses and the provided helper
functions, including the NodeVisitor and NodeTransformer. I will finish by
talking about how the ast module can be used to analyze Python code and how it
can be used to generate new code.

I expect the time to break down roughly like this:

Introduction ( 5m )

  * Capacitor joke 
  * What is an abstract syntax tree? 
  * How they are used by the Python interpreter 

The contents of the ast module (20 m)

  * The node subclasses and the ast ( 10m ) 
    * How you get an ast. 
      * code examples
    * ast.stmt vs. ast.expr 
    * peculiarities 
      * code examples 
        * elif as syntactic sugar for "if: else: if:" 
        * comparison operators 
    * Why this is useful. 
      * the ast is the "truth" of the program 
        * code examples 
        * tricky code 
  * The ast module helpers ( 10m ) 
    * visitor pattern 
    * NodeVisitor 
    * NodeTransformer 
    * code examples 

What you do with an ast ( 15m )

  * Walking an ast 
    * code examples 
      * a simple visitor to gather variables by scope
  * Creating/Modifying an ast 
    * code examples 
      * rearrange imports transformer 
      * naive "rename all instances" transformer 
      * naive macro expansion transformer 

Conclusion ( 5m )

  * Practical Applications 
    * existing projects 
      * visitors 
        * checkers (pylint, pyflakes)
      * transformers 
        * refactoring tools (rope)
  * When is it a good idea to use ast? 
