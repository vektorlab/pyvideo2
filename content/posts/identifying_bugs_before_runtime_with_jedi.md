---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=DfVHSw0iOsk"'
Speakers: [Dave Halter]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/DfVHSw0iOsk/hqdefault.jpg'
Title: '"Identifying Bugs Before Runtime With Jedi"'
date: '2014-07-23'
---
Jedi is an autocompletion library for Python that has gained quite a following over the last year. There are a couple of plugins for the most popular editors (VIM, Sublime, Emacs, etc.) and mainstream IDEs like Spyder are switching to Jedi.

Jedi basically tries to redefine the boundaries of autocompletion in dynamic languages. Most people still think that there's no hope for decent autocompletion in Python. This talk will try to argue the opposite, that decent autocompletion is very close.

While the first part will be about Jedi, the second part of this talk will discuss the future of dynamic analysis. Dynamic Analysis is what I call the parts that static analysis doesn't cover. The hope is to generate a kind of "compiler" that doesn't execute code but reports additional bugs in your code (AttributeErrors and the like). 

I still have to work out the details of the presentation. I also have to add that Jedi I'm currently working full-time on Jedi and that there's going to be some major improvements until the conference. Autocompletion and static/dynamic analysis as well as refactoring are hugely important tools for a dynamic language IMHO, because they can improve the only big disadvantage compared to static languages: Finding bugs before running your tool.