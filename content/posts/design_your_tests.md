---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=xkwBjsjSERU"'
Speakers: [Julian Berman]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/xkwBjsjSERU/hqdefault.jpg'
Title: '"Design Your Tests"'
date: '2014-07-23'
---
* Life span of a test
    * 5 minute - why does this fail?
    * 5 day - what is this missing?
    * 5 week - do I have coverage for this?
    * 5 month - what's *not* causing this bug?

* Transparent simplicity
    * one or two "iceberg" layers for meaning
        * Higher-order assertions - build collections of state that have meaning for the domain in the tests
        * bulk of the details are in the code itself

        * show an example

    * grouping for organization
        * Mixins

        * show an example

* unittest issues
    * assertion/mixin clutter
    * setUp/tearDown tie grouping to the class layer or to inheritance via super
        * addCleanup
    * weak association / lookup-ability between code and its tests
        * package layout
        * other conventions

* Alternative approaches
    * testtools' matchers
    * py.test `assert` magic