---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=1ABPQyANid0'
Speakers: [Tom Eastman]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/1ABPQyANid0/hqdefault.jpg'
Title: 'The one true way of doing Django deployments...'
date: '2015-08-04'
---
...doesn't exist. (Sorry)

The power and flexibility of Django comes with drawbacks. One of the toughest for project management is working out how to deploy your Django application. If you ask five different authorities on how you should do it, you'll get six different answers.

And if someone says "Just use fabric!": they're not helping.

Release management, dependency wrangling, virtualenv care and feeding; to .whl or .deb? To containerize or Heroku-ize? Do you really have to allow your servers unconstrained Internet access just to build your virtualenv?

As a Django user, you might end up writing more deployment solutions than Django projects. I know I have.

There's no one true way of doing Django deployments, but some work better than others. Maybe I can show you.