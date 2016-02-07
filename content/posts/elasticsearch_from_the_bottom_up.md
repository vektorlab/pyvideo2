---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=PpX7J-G2PEo'
Speakers: [Alex Brasetvik]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/PpX7J-G2PEo/hqdefault.jpg'
Title: 'Elasticsearch from the bottom up'
date: '2014-07-24'
---
## Who I am and motivation
I work with hosted Elasticsearch and have interacted with lots of developers. We see what many struggle with.

Some relevant theory helps a lot. What follows has already lead to many "Aha!"-moments and developers piecing things together herself.

## The inverted index
The most important index structure is actually very simple. It is essentially a sorted dictionary of terms, with a list of postings per term.

We show three simple sample documents and the resulting inverted index.

## The index term
The index term is the "unit of search", and the terms we make decide how we can search.

With the inverted index and its sorted dictionary, we can quickly search for terms given their prefix.

## Importance of text analysis
Thus, we need to transform our search problems into string prefix problems.

This is done with text analysis, which is the process of making of index terms. It is highly important when implementing search.

## Building indexes
The way indexes are built must balance how compact an index is, how easily we can search in it, how fast we can index documents - and the time it takes for changes to be visible.

Lucene, and thus Elasticsearch, builds them in segments.

## Index segments
A Lucene index consists of index segments, i.e. immutable mini-indexes.

A search on an index is done by doing the search on all segments and merging the results.

Segments are immutable:

This enables important compression techniques.
Deletes are not immediate, just a marker.
Segments are occasionally merged to larger segments. Then documents are finally deleted.
New segments are made by buffering changes in memory, and written when flushing happens. Flushes are largely caused by refreshing every second, due to real time needs.

## Caches
Caches like filter- and field caches are managed per segment. They are essential for performance.

Immutable segments make for simple reasoning about caches. New segments only cause partial cache invalidations.

## Elasticsearch indexes
Much like a Lucene index is made up of many segments, an Elasticsearch index is made up of many Lucene indexes.

Two Elasticsearch indexes with 1 shard is essentially the same as one Elasticsearch index with 2 shards.

Search all shards and merge. Much like segments, but this time possibly across machines.

Shard / Index routing enables various partitioning strategies. Simpler than it sounds, so one important example:

Essential for time based data, like logs: can efficiently skip searching entire indexes - and roll out old data by deleting the entire index.

## Common pitfalls
We must design our indexing for how we search - not the searches for how things are indexed. Be careful with wildcards and regexes.

Since segments are immutable, deleting documents is expensive while deleting an entire index is cheap.

Updating documents is essentially a delete and re-index. Heavy updating might cause problems.

Have enough memory and then some. Elasticsearch is very reliant on its caches.

## Summary
We've seen how index structures are used, and why proper text processing is essential for performant searches.

Also, you now know what index segments are, and how they affect both indexing and searching strategies.

## Questions