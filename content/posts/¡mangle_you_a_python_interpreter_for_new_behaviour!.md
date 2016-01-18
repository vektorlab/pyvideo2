---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=9_LnOTFDNUk"'
ThumbnailUrl: 'https://i.ytimg.com/vi/9_LnOTFDNUk/hqdefault.jpg'
date: '2015-08-16'
speakers: [Javier Candeira]
tags: []
---
What happens when you feel some syntax or behaviour is missing from Python? You could fork the interpreter, but then nobody else could run your programs. Instead, you could implement the new behaviour as a Python module to be imported, and distribute it with your programs.

Following hot on the tracks of previous Pycon-AU talks like "Don't Do This" (2013) and the "ugly hacks" bit of "Here be dragons: some elegant and ugly hacks in CPython" (2014), this presentation will grant some of the requests you never dared to make:

- You'd like for PEP 336, Make None Callable to have succeeded? You can make your own None()! Easy in CPython with CTypes!

- You'd like to have the "?." operator available for safe attribute access? Just add the syntax to pypy, then use a source codec hack to rewrite it into a legal Python 2.7 function. Too easy!

- Your reaction to all of this is “please make it stop”? The talk will finish by discussing why having extensible syntax as a standard Python feature might even be a good idea! It is in other languages!

This talk is for intermediate to advanced Python users, and for beginning Python implementors.

Slides: http://hiperactivo.com/talks/pyconau15/mangling_python/

Repos:

  - quiet_None: https://bitbucket.org/candeira/quiet_none/

  - question_dot: https://bitbucket.org/candeira/question_dot/

