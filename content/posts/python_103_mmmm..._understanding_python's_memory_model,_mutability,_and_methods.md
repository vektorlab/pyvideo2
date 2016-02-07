---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=HHFCFJSPWrI'
Speakers: [wesley chun]
Tags: [debugging, exceptions, memory, scripts]
ThumbnailUrl: 'http://i.ytimg.com/vi/HHFCFJSPWrI/hqdefault.jpg'
Title: 'Python 103: Mmmm... Understanding Python''s Memory Model, Mutability, and
  Methods'
date: '2011-07-21'
---
In Python 101, you learned basic Python syntax, what its flow control
mechanisms and basic data types are and how they work. You learned how to
write functions and developed executable Python scripts that actually work!
You probably also learned how to create files, how to open, read from or write
to them, and close them. Perhaps you've even learned a little bit of object-
oriented programming, developed a couple of Python classes, most with user-
defined methods, and have no problems creating instances to use in your
applications.

In Python 102 (or equivalent in experience), you explored further, using
default values and variable arguments for functions, discovered how to catch
exceptions and write handlers for them… perhaps you've even created your own
exceptions. You have found some useful Python standard library modules and
using them actively in your own applications. You've quite comfortable with
OOP, creating classes and using instances regularly in your programs. In fact,
you've been coding Python for 6 months to a couple of years now. You're much
more serious about Python now because you're no longer a "beginner." You've
even taken notice at the growing number of jobs requesting or requiring Python
skills.

As an aspiring Python developer, you are starting to be more aware of the
entire ecosystem around you, and think you may be ready for "prime-time" and
feel able to take on a full-time position as a Python programmer. However, if
you have experienced one or more of the below questions or problems, this talk
may be for you:

  * Throughout this time, you've experienced strange bugs in your code. In particular, you notice that things don't always behave the way you expect and have spent a good amount of time debugging various parts of your software that you thought were actually correct - you work around them but are disturbed and don't have the time nor committment to fully investigate.

  * You've created classes and objects just fine but wish that you could use some of Python's operators (like +, in, len(), etc.) with your objects, which feel like they're "2nd-class" citizens compared to the standard data types.

  * Do you know what functional evaluation strategy means? Have you been asked or considered whether Python is "call-by-value" or "call-by-reference"? It is important to you, and can you clearly explain your answer?

  * What does "mutability" mean? What is the difference between mutable and immutable objects? Which Python objects are mutable and which aren't?

  * Can you clearly explain both the output in the two code snippets below, and even more importantly, _why_ the output is the way it is?

SNIPPET A x = 42 y = x x += 1 print x print y

SNIPPET B x = [1, 2, 3] y = x x[0] = 4 print x print y

  * Have you seen odd behavior in container or collection objects like lists or dictionaries? For example, you may have copied those types of objects and discovered weird things happening to both the original and the copy, or that you seen something not quite right if you loop through it and remove items from it. 

This is what Python 103 is for… to fill in all the missing gaps, to answer all
the questions (including those above) that do not seem to have easy-to-find
answers on Google, but only if you have the desire to learn more about the
interpreter to take your Python skills to the next level.

