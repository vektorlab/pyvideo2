---
Category: 'PyCon AU 2014'
Copyright: 'http://www.youtube.com/t/terms'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=LrW-HSHP0ws"'
Speakers: [Tom Eastman]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/LrW-HSHP0ws/hqdefault.jpg'
Title: '"Serialization formats aren''t toys by Tom Eastman"'
date: '2014-08-07'
---
Do you have an API? 

Do you accept input from users? Do you accept it in XML? What about YAML? Or maybe JSON? How safe are you?

Are you sure?

It’s not in the OWASP Top 10, but you don’t have to look far to hear stories of security vulnerabilities involving deserialization of user input. Why do they keep happening?

In this talk I’ll go over what the threat is, how you are making yourself vulnerable and how to mitigate the problem. I’ll cover the features (not bugs, features) of formats like XML, YAML, and JSON that make them surprisingly dangerous, and how to protect your code from them.

Because here’s the thing: If you are using, say, a compliant, properly implemented XML parser to parse your XML, you are NOT safe. Possibly quite the opposite.