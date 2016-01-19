---
Category: 'Kiwi PyCon 2015'
Copyright: 'CC BY-SA'
Language: 'English'
SourceUrl: '"http://youtu.be/fM5d_2BS6FY"'
Speakers: [Robert Collins]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/fM5d_2BS6FY/hqdefault.jpg'
Title: '"Functionalish programming in Python with effect"'
date: '2015-09-05'
---
'everyone' knows that separating out IO and other side effects makes code easier to unit test. What if there were a Python library that helps do that systematically which you could use to make all your things better? There is. Come and find out more.

Chris Armstrong's Effect library is the library in question. I found this while digging into all the varied implementations of monads for Python (a generic concept that encapsulates the principle of IO and side effects) - and I'd like to share its beauty with other folk. Effect (https://pypi.python.org/pypi/effect) allows consistent separation of side effect (e.g. IO or even just global state changes) from the code that depends on those effects. Testing and reasoning about code becomes easier. But it can often be hard to get into such a system. Allow me to take you on a tour through how to change regular code into super testable code using Effect.