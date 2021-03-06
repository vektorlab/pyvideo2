---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=1i5leCslA4g'
Speakers: [Christopher Neugebauer]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/1i5leCslA4g/hqdefault.jpg'
Title: 'Test-Driven Repair'
date: '2015-08-04'
---
“it is impossible BY DEFINITION to do Test-Driven Development after the code is written.” — Tim Ottinger, author of ‘Clean Code’, on Twitter [1].

Automated testing is one of the most important tools in the modern programming toolbox: good tests help you find regressions early, and help you make sure your code is right before it ships. Test-driven development is a great way to make sure your software is up to specification before you start work. Even better, it makes sure your software’s architecture is amenable to writing tests from day 1.

So what happens when you find yourself working on code where automated testing took a back seat to being shipped? Chances are you’ll have a sea of bugs, strung together in a structure where writing simple unit tests just isn’t going to happen.

Broken code is a support burden, and if it’s in production, you’ve got no choice but to make things work. Luckily, automated testing isn’t a lost cause here!

In this talk, we’ll look at how to approach automated testing on late-stage, or even production code… or in any situation when you don’t have the luxury of starting with a test-driven structure. We’ll look at techniques that I’ve used to analyse faults in existing code, and how to translate those into tests, and how to use that to fix bugs.

In particular, we’ll look at:

- Tooling and metrics to help you decide what code to test, and how to measure progress when you’re writing tests
- Approaches to constructing test cases for old code, including using data-driven approaches, and approaches based on requirements specifications
- Granularity — making tests on old code granular enough is difficult, so we’ll look at the trade-offs between unit and integration tests on old code, and ways to make integration-level tests granular enough to make results reliable

We’ll see that testing old code is both achievable, and actually a worthwhile exercise. You’ll find bugs. You’ll increase quality. You’ll make your code more maintainable! Do try it!

[1] https://twitter.com/tottinge/status/544632253205475329
