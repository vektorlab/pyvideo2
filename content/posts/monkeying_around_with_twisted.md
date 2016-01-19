---
Category: 'PyCon ZA 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://archive.org/details/pyconza2014-monkeying-with-twisted"'
Speakers: [Richard Spiers]
Tags: [pyconza, pyconza2014]
ThumbnailUrl: 'http://archive.org/download/pyconza2014-monkeying-with-twisted/pyconza2014-monkeying-with-twisted.thumbs/11%20B%20Monkeying%20around%20with%20Twisted-_001470.jpg'
Title: '"Monkeying around with Twisted"'
date: '2014-10-03'
---
Twisted is an open source framework for writing network based services. It utilises an asynchronous, event driven model which allows the rapid development of custom network protocols. While Twisted makes implementing network services much easier, it comes with its own set of challenges. One of these challenges involves tracking the context of multiple requests. In a traditional web server the thread ID could be used to track a particular request and modify log entries appropriately. However, this does not work in Twisted as it utilises a single thread (generally speaking).
We have chosen to tackle this issue, amongst others, by monkey patching some of the Twisted subsystems.
Through this talk we will introduce Twisted as a viable option for programming network based services. No previous Twisted knowledge is required, and the concepts introduced will be explained through real world examples of restful controllers implemented in Twisted. This primer will be followed by a discussion on our solution to the context tracking problem as well as some of the other areas in which we have found monkey patching to be beneficial.