---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=NZnnB7l3ZHM'
Speakers: [Erik Rose]
Tags: [django, nose, testing]
ThumbnailUrl: 'http://i.ytimg.com/vi/NZnnB7l3ZHM/hqdefault.jpg'
Title: 'Django''s Nasal Passage'
date: '2012-09-06'
---
  * Why nose?
    * Pain points with standard Django testing
    * Extensibility without writing custom, uncombineable testrunner subclasses
    * Rich ecosystem of helpful plugins
  * django-nose
    * Testing just your apps, not all the random installed stuff
    * Test-selection tricks: running just failed tests, running a module, etc.
    * Killing the boilerplate:
      * No more imports into **init**
      * No more class name collisions and accidental shadowing
      * With all this freedom, how best should you organize your tests?
    * Going 4 times faster with fixture bundling
      * Troubleshooting
      * Fixtures are evil
      * Where do I put the factories?
    * Speeding startup with test DB reuse
    * Writing faster TransactionTestCases with hygienic base classes
      * Background on Django's handling of TransactionTestCases
      * How to improve matters
    * Test-only models: what's the best practice?
  * nose-progressive
    * Dots considered harmful. When will my tests be done?
    * Patience is for the dead. Show me my tracebacks as they happen!
    * My terminal is only this big. Don't waste my space.
    * Hiding pointless stack frames
    * Editor round-tripping for quick debugging
  * Splitting into sub-suites
    * An introduction to the attr plugin
    * Have some run only on CI machines, some constantly, others before checkin
    * Choosing tests with regexes
  * Other fun plugins
    * f7u12, for when your tests get angry
    * Coverage
    * xunit, for your continual integration pleasure
    * Profiling

