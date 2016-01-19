---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=L6TtXrLmdKA"'
Speakers: [Schlomo Schapiro]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/L6TtXrLmdKA/hqdefault.jpg'
Title: '"DevOps Risk Mitigation: Test Driven Infrastructure"'
date: '2014-07-23'
---
Common wisdom has it that the test effort should be related to the risk of a change. However, the reality is different: Developers build elaborate automated test chains to test every single commit of their application. Admins regularly “test” changes on the live platform in production. But which change carries a higher risk of taking the live platform down?

What about the software that runs at the “lower levels” of your platform, e.g. systems automation, provisioning, proxy configuration, mail server configuration, database systems etc. An outage of any of those systems can have a financial impact that is as severe as a bug in the “main” software!
One of the biggest learnings that any Ops person can learn from a Dev person is Test Driven Development. Easy to say - difficult to apply is my personal experience with the TDD challenge.

This talk throws some light on recent developments at ImmobilienScout24 that help us to develop the core of our infrastructure services with a test driven approach:

* How to do unit tests, integration tests and systems tests for infrastructure services?
* How to automatically verify Proxy, DNS, Postfix configurations before deploying them on live servers?
* How to test “dangerous” services like our PXE boot environment or the automated SAN mounting scripts?
* How to add a little bit of test coverage to everything we do.
* Test Driven: First write a failing test and then the code that fixes it.

The tools that we use are Bash, Python, Unit Test frameworks and Teamcity for build and test automation.

See http://blog.schlomo.schapiro.org/2013/12/test-driven-infrastructure.html for more about this topic.
