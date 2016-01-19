---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=SGleKfigMsk"'
Speakers: [Graham Dumpleton]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/SGleKfigMsk/hqdefault.jpg'
Title: '"Using benchmarks to understand how WSGI servers work"'
date: '2015-08-03'
---
During the development of a Python web application the inbuilt development web server provided by the web framework is often what is used. When moving to a production environment, one has to choose a more capable production grade WSGI deployment mechanism. Which of the various WSGI servers available is going to be the most suitable is going to depend on a range of criteria related to your specific web applications requirements.

Unfortunately, rather than look at the bigger picture and what would be the most suitable across such criteria, many people will simply rush to trying to run an overly simplistic benchmark on the various WSGI servers and make the decision based purely on perceptions of whether one WSGI server is faster than the alternatives. Worse, they don't even attempt to do the benchmarks themselves and instead rely on benchmarks published on some public blog site.

Such public benchmarks as are available are often flawed, or cover such a narrow use case as to in no way be relevant to that users own specific situation.

A further problem with such benchmarks is that they try and evaluate the performance of a WSGI server as if they are a black box. As such, there is no attempt to try and work out what is actually going on within the WSGI server and why it is exhibiting the behaviour it is.

The purpose of this talk is to explore a number of different micro benchmarks, using them to work out what is actually going on within a WSGI server when they are run. The analysis will delve down into, and look at the different ways that WSGI servers are implemented and deployed. The behaviour under the different benchmarks will be determined using fine grained metrics captured from hooking instrumentation into the WSGI servers themselves.

As there are many factors which could be investigated, the talk cannot be entirely comprehensive, but selected benchmarks drawing from a sub set of the following areas will be presented:

* multithreading
* CPU intensive tasks
* long running requests
* combination of short and long running requests
* large request content uploads
* large amounts of response content
* blocking on back end services
* slow HTTP clients

The tests will look not just at response times, but also server capacity utilisation, CPU and memory utilisation.

Although the discussion will primarily revolve around WSGI servers, a comparison will also be made for some tests were one instead to use an ASYNC web application framework alone, or in conjunction with a WSGI adapter.

To conclude, an attempt will be made to summarise what you should be looking at in a WSGI server to determine if it is the right choice for your use case.