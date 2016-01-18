---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=NvV5OrVk24c"'
ThumbnailUrl: 'http://i.ytimg.com/vi/NvV5OrVk24c/hqdefault.jpg'
date: '2014-07-23'
speakers: [Austin Bingham]
tags: []
---
Python is a modern, dynamic language which is growing in popularity, but tool support for it is sometime lacking or only available in specific environments. For refactoring and other common IDE functions, however, the powerful open-source rope library provides a set of tools which are designed to be integrated into almost any programming environment. Rope supports most common refactorings, such as renaming and method extraction, but also more Python-specific refactorings, such as import organization. Rope’s underlying code analysis engine also allows it to do things like locating method definitions and generating auto-completion suggestions.

While rope is designed to be used from many environments, it’s not always easy or ideal to integrate rope directly into other programs. Traad  (Norwegian for “thread”) is another open-source project that addresses this problem by wrapping rope into a simple client-server model so that client programs (IDEs, editors, etc.) can perform refactorings without needing to embed rope directly. This simplifies dependencies, makes clients more robust in the face of errors, eases traad client development, and even allows clients to do things like switch between Python 2 and 3 refactoring in the same session.

In this session we’ll look at how rope operates, and we’ll see how traad wraps it to provide an easier integration interface. The audience will get enough information to start using rope themselves, either directly or via traad, and they’ll see how to use traad for integrating rope into their own environments. More generally, we’ll look at why client-server refactoring tools might be preferable to the more standard approach of direct embedding. 
