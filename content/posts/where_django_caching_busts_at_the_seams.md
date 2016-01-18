---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=dXDLWGY0Tro"'
ThumbnailUrl: 'http://i.ytimg.com/vi/dXDLWGY0Tro/hqdefault.jpg'
date: '2012-09-06'
speakers: [Kyle Rimkus, Mike Biglan]
tags: [caching, django]
---
Most mid-sized Django websites thrive by relying on memcached. Though what
happens when basic memcached is not enough? And how can one identify when the
caching architecture is becoming a bottleneck? We'll cover the problems we've
encountered and solutions we've put in place.

The following highlight the issues we'll discuss during the talk:

  * Cache Warming. For content that will likely be in demand, getting it ready in cache before use is a helpful start. 
  * Two-tier caching. In multi-server environments, certain content that changes infrequently and has high-demand can be cached locally on each server. In these cases, having methods to burn the cache on each server becomes critical.
  * Categorizing Cache. If good estimates exist for the expected demand of certain cache as well as the frequency of change, this can lead to better insight into when to warm that content as well as whether to cache it locally.
  * Caching comparison with memcached vs. reddis vs. mongo
  * Cachemodel. Our open-source, mini-framework for simplifying caching in Django. 
  * Adding servers to memcached. And consistent hashing algorithms to avoid having to burn all cache when the cache cluster changes in size.
  * Elasticache on AWS.

As caching problems become more common, better layers and mini-frameworks will
help simplify and elegantly solve some of these problems.

