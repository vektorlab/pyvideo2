---
Category: 'PyCon ZA 2015'
Copyright: ''
Language: 'English'
SourceUrl: 'http://youtu.be/3u6ZH4ntp-0'
Speakers: [Stefano Rivera]
Tags: [room 215]
ThumbnailUrl: 'https://i.ytimg.com/vi/3u6ZH4ntp-0/hqdefault.jpg'
Title: 'The Road to Continuous Deployment'
date: '2015-10-02'
---
How do we get work from a developer's laptop to a production server?
How do we do this repeatedly? How do we avoid releasing bad patches? How do we get changes out as fast as possible? And what happens to requests during a deploy? If you want continuous deployment, you have to solve these problems.

How do you handle configuration, so that the same code can run in multiple environment? From a developers laptop, to QA environments, to production. What about the quirks of each machine in production?

This talk will look at the path Yola took, with Jenkins, yoconfigurator, yodeploy. It's by no means a complete solution, but it's good enough that I rarely find myself working on it, these days.

We will cover the pros and cons of each path one can take. The whole platform architecture is really affected by this. We can talk about: Bare hardware, virtualization, containerization, build systems, linux distributions packages, language package ecosystems, configuration management systems, notifications, secret distribution, and much more.
