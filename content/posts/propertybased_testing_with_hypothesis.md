---
Category: 'PyCon ZA 2015'
Copyright: ''
Language: 'English'
SourceUrl: '"http://youtu.be/mg5BeeYGjY0"'
ThumbnailUrl: 'https://i.ytimg.com/vi/mg5BeeYGjY0/hqdefault.jpg'
date: '2015-10-02'
speakers: [Jeremy Thurgood]
tags: [Room 215]
---
Unit testing can be more effective and less tedious when you have an army of robot monkeys at your disposal. Why should humans have to worry about finding the particular combination of Turkish and Tengwar that crashes the serialiser, or the convoluted sequence of operations that corrupts the database?

>     Hypothesis is a Python library for turning unit tests into generative tests,
>     covering a far wider range of cases than you can manually. Rather than just
>     testing for the things you already know about, Hypothesis goes out and
>     actively hunts for bugs in your code. It usually finds them, and when it
>     does it gives you simple and easy to read examples to demonstrate.
>
> -- Hypothesis 1.0 release announcement

Property-based testing lets you think about your tests in terms of general behaviour and invariant properties instead of getting lost in the details of individual examples, and good tools (such as <a href="https://hypothesis.readthedocs.org/en/latest/">Hypothesis</a>) will explore quite complex combinations of test data and reduce them to minimum failing cases.

This talk will provide a practical introduction to property-based testing with Hypothesis, and show how you can use it to build more effective test suites with less effort.