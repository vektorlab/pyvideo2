---
Category: 'Kiwi PyCon 2013'
Copyright: ''
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=WSdyU5s-SMI'
Speakers: [Ryan Kelly]
Tags: []
ThumbnailUrl: 'http://i1.ytimg.com/vi/WSdyU5s-SMI/hqdefault.jpg'
Title: 'Testing for Graceful Failure with Vaurien and Marteau'
date: '2013-09-12'
---
@ Kiwi PyCon 2013 - Sunday, 08 Sep 2013 - Track 2

**Audience level**

Intermediate

**Abstract**

So you've built an awesome webapp, put it through its paces, and assured yourself that it does what it's supposed to do. Great! Now how does it behave when things start to go wrong?

This talk will demonstrate how the Mozilla Services team tests for failure scenarios in our web services, focusing on two key python-based tools: Marteau, a web-based frontend for easily running load-tests and analyzing the results, and Vaurien, a misbehaving TCP proxy that can simulate a variety of backend failure modes.

Used together, these tools can help ensure that a web service will not only scale up to meet its expected demand, but will fail gracefully when it finally reaches breaking point.

The talk will cover:

 * Real-life examples of bugs that only show up when your app is under load; bugs that can turn a brief partial outage into a cascading whole-system failure.
 * The basics of writing a load-testing suite for your app.
 * How to set up Marteau for easy on-demand load testing.
 * How to use Vaurien to simulate various kinds of backend failure, such as an overloaded database, misconfigured DNS, or a suddenly-disappearing job queue.
 * Some tips for systematically applying these tools to your own setup.

**Slides**

https://speakerdeck.com/nzpug/ryan-kelly-testing-for-graceful-failure-with-vaurien-and-marteau
