---
Category: 'PyCon AU 2014'
Copyright: 'http://www.youtube.com/t/terms'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=Yk5EE0Us0DE'
Speakers: [Graham Dumpleton]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/Yk5EE0Us0DE/hqdefault.jpg'
Title: 'How do debug tool bars for web applications work? by Graham Dumpleton'
date: '2014-08-11'
---
When your production web application breaks, working out what went wrong can be hard. Information from log messages and details of any Python exceptions which occurred, along with other application performance data can help to identify the issue, but not always. Often you will need to fall back to a development or test environment and hope you can replicate the problem and then debug the issue from there.

The purpose of this talk is to dive in and look at one class of tools that can be used in helping debug web applications. Specifically, it will look at web application tools such as the Django debug tool bar.

Rather than simply look at how you might use such a tool though, this talk will look at how these debug tool bars are actually implemented, how they hook into your web application, how they capture the information that they do, as well as how they can be extended to add new functionality.

The limitations on these tools as far as performance overhead, security of data etc, which nearly aways lead to them only being recommended for development environments, will also be discussed.

At the same time though, this notion that they are only suitable for development environments will also be challenged by looking at how a tool such as the New Relic Python agent, which implements application performance monitoring, overcomes such limitations to provide a production grade solution.

Are there lessons to be learnt from how the New Relic Python agent works which could drive improvements to existing web application debug tool bars? Could the New Relic Python agent itself be used as a base for a new generation of debug tool bars which combine an ability to debug a web application, even in a production environment, with the ability to monitor the performance of the web application over time?
