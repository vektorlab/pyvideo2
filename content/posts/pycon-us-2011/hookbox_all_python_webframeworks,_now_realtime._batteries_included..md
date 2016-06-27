---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/371_hookbox-all-python-web-frameworks-now-real-time-batteries-included.mp4
Speakers: [Michael Carter]
Tags: [hookbox, pycon, pycon2011, realtime, webapps]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011HookboxAllPythonWebframeworksNowRealtimeBatteri858.png'
Title: 'Hookbox: All Python web-frameworks, now real-time. Batteries Included.'
date: '2011-03-11'
---
Hookbox: All Python web-frameworks, now real-time. Batteries Included.

Presented by Michael Carter

Learn how to supercharge your python web applications (Django, Pylons, TG,
GAE, Werkzeug, WSGI, etc) with real-time features! Presenceful and moderated
chat? About 10 minutes, seriously. A real-time graph to monitor the CPU? Less
than five. If you pay attention for at least half of this talk, you'll leave
confident and ready to take advantage of WebSocket, Comet, and the world,
thanks to Hookbox.

Abstract

Hookbox ([http://hookbox.org](http://hookbox.org/)) is a Python and Eventlet-
based Comet-server/message-queue which tightly integrates with existing web
application infrastructure via web hooks and a REST interface; Hookbox’s
purpose is to ease the development of real-time web applications, with an
emphasis on tight integration with existing web technology. Put simply,
Hookbox is a web-enabled message queue.

Browers may directly connect to Hookbox, subscribe to named channels, and
publish and receive messages on those channels in real-time. An external
application (typically the web application itself) may also publish messages
to channels by means of the Hookbox REST interface. All authentication and
authorization is performed by an external web application via designated
“webhook” callbacks.

In this talk we cover the broad principles of Hookbox, then examine a few
short examples in depth, including presenceful and moderated chat, real-time
graphing, and, of course, a game. The code examples are very purposefully
brief; the important parts of the talk deal with the interaction model between
browser, web framework, and Hookbox -- everything else follows naturally and
easily into place.

The audience need not be familiar with a particular web framework over
another, but they must be proficient with at least one.

Though this talk is aimed at a novice level, we'll also spend some time
talking about the more advanced features that Hookbox provides.
