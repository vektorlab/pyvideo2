---
Category: 'PyCon AU 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=bIWnQ3F1eLA'
Speakers: [Tom Eastman]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/bIWnQ3F1eLA/hqdefault.jpg'
Title: 'Caching: A trip down the rabbit hole by Tom Eastman'
date: '2014-08-11'
---
The question: How do I make my website fast?

If that sounds like a loaded question to you: good, we're on the same page.

In this talk I will give you a full overview of one of the most powerful and headache-inducing tools in the web-developer's kit: caching.

This is a talk for all experience levels, from beginner to seriously brain-melty. The code and scenarios we'll be exploring are within the context of a Django project, but the principles are applicable to all of web development.

We'll begin our journey in the light, warm land of web browser caches: learning how you can make your users' web browsers do all the work for you. Making your site feel rocket-fast and responsive with little more than some finely crafted HTTP response headers.

From there, we'll begin our descent into the underworld of server-level caching, using reverse-proxies such as Varnish or Nginx that shield the application code from having to do any work. What they do, how they can help, and more important -- when do they *not* help, and when do you have to go deeper.

Finally we'll explore the dark art of application-level caching. Whether it's caching whole responses, partial responses, preventing repetitive SQL queries or expensive API response serialization calls. And, if our brains haven't exploded yet, we might throw in some asynchronous cached-view-generation  just for good measure.

Whether you're a hobbyist or a grizzled veteran, you should come out of this talk with a few new tricks up your sleeve for making all your sites do more with less work.

Expect references from -- depending on mood -- Alice in Wonderland, The Matrix, or Dante Alighieri's "Inferno".
