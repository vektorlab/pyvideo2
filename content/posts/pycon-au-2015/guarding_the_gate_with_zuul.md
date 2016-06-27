---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=HlpJhqgGL34'
Speakers: [Joshua Hesketh]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/HlpJhqgGL34/hqdefault.jpg'
Title: 'Guarding the gate with Zuul'
date: '2015-08-04'
---
Zuul is a program that is used to gate the source code repositories of a project so that changes are only merged if they pass tests.

By gating we mean a more proactive continuous integration suite whereby tests must pass in order to merge (rather than a traditional CI that just gives a nightly status of the master branch). This means every commit is tested both during review time and before it merges - in case the repositories have changed in the mean time.

The result of using a gating system like zuul is that it's much harder to break trunk and your nightly builds should nearly always work.

Zuul can be configured to react to events and run various jobs with success or failure results depending on the scenario. Currently Zuul is only integrated with the gerrit code review platform but there are discussions about extending it to github.

One unique and powerful feature in Zuul is its ability to run tests in a predictive manner across multiple programs. Zuul predicts what multiple repositories will look like by the time the present job is finished and arranges the tests to be performed in that order. This stops race conditions when merging code in one repository that depends on code in another repository.

Zuul can manage thousands of jobs across hundreds of projects as evident by being the gate keeper for OpenStack.

In this talk we will look at what Zuul is, how to configure it and the internals of how it works.
