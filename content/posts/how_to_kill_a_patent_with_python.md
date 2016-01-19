---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/425_how-to-kill-a-patent-with-python.mp4
Speakers: [Van Lindberg]
Tags: [casestudy, patents, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011HowToKillAPatentWithPython889.png'
Title: '"How to kill a patent with Python"'
date: '2011-03-11'
---
How to kill a patent with Python

Presented by Van Lindberg

Finding the right piece of "prior art" - technical documentation that
described a patented piece of technology before the patent was filed - is like
finding a needle in a very big haystack. This session will talk about how I am
making that process faster and more accurate through the use of natural
language processing, graph theory, machine learning, and lots of Python.

Abstract

From my work consulting on a number of patent cases, I am frequently asked to
find "prior art" - patents and publications that describe a technology before
a certain date. The problem is that the indexing mechanisms for patents and
publications are not as good as they could be, making good prior art searching
more of an art than a science. When I decided to do better, I reached for
Python.

  * Part I (5 mins): The USPTO as a data source.* The full-text of each patent is available from the USPTO (and now from Google.) What does this data look like? How can it be harvested and normalized to create data structures that we can work with? 
  * Part II (15 mins, in two parts):* Once the patents have been cleaned and normalized, they can be turned into data structures that we can use to evaluate their relationship to other documents. This is done in two ways - by modeling each patent as a document vector and a graph node. 
  * Part IIA (7 mins): Patents as document vectors.* Once we have a patent as a data structure, we can treat the patent as a vector in an n-dimensional space. In moving from a document into a vector space, we will touch on normalization, stemming, TF/IDF, Latent Semantic Indexing (LSI) and Latent Dirichlet Allocation (LDA). 
  * Part IIB (7 mins): Patents as technology graphs.* This will show building graph structures using the connections between patents - both the built-in connections in the patents themselves as well as the connections discovered while working with the patents as vectors. We apply some social network analysis to partition the patent graph and find other documents in the same technology space. 
  * Part III (5 mins): What have we built?* Now that we have done all this analysis, we can see some interesting things about the patent database as a whole. How does the patent database act as a map to the world of technology? And how has this helped with the original problem - finding better prior art?

