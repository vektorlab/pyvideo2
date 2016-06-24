---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=zqRd941NXlI'
Speakers: [Nathan Craike]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/zqRd941NXlI/hqdefault.jpg'
Title: 'Fang: Pythonic dependency injection'
date: '2015-08-04'
---
Dependency injection (DI) is a technique most often used in "big OO" languages like Java and C#. It's usually dismissed by Python developers as only needed because of these other languages' deficiencies: static typing, restrictive object systems, lack of reflection, etc.

However, there are other dynamically-typed languages which do use forms of dependency injection. From looking at these systems, we can see there are some advantages to dependency injection _even if_ you're not using a traditional "big OO" language with static types and interfaces. Dependency-injected code can be more modular, much easier to test, easier to analyse, and easier to modify or extend to meet new requirements.

Despite this, there aren't many dependency-injection systems for Python. The few that do exist aren't "Pythonic", or implement DI in ways that compromise a lot of its benefits.

Fang is a library which adds dependency injection to Python in a way which provides real benefits for code clarity, ease of testing, and maintainability, while still fitting naturally into Python's idioms. Fang describes dependencies concisely but explicitly, and doesn't restrict the developer to a particular paradigm on how dependencies are validated or met.

This talk will give a brief overview of how DI is used across a few languages (both traditional OO and dynamic languages) and highlight what elements of DI can be beneficial in Python. The talk will then demo how Fang can be used to add DI to Python code, and show some of the benefits to code clarity, unit testing and code analysis.

