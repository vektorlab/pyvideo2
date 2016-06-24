---
Category: 'Kiwi PyCon 2013'
Copyright: ''
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=CxK-v0pSpjo'
Speakers: [Alan Williams]
Tags: []
ThumbnailUrl: 'http://i1.ytimg.com/vi/CxK-v0pSpjo/hqdefault.jpg'
Title: 'Computational Advertising, Billions of records, and AWS - Lessons Learned'
date: '2013-09-12'
---
@ Kiwi PyCon 2013 - Sunday, 08 Sep 2013 - Track 2

**Audience level**

Experienced

**Abstract**

Overview - hope this will be useful, but caveat emptor - not a how-to, that's well covered elsewhere - problem - recovering value from large web logs - user targeting

Is this Big Data? - When should you think about Hadoop - AWS servers available with 244 GB of memory - Twitter WTF paper, Microsoft cluster utilisation paper

Logging, Storing, and Munging - Looked at EMR but (1) it's hard to log (2) versioning issues. - For on-demand use CM is good - For automated use, combination of CDH, whirr, and boto. - backing up HBase and HDFS to S3

Processing the data - hadoop as solving distributed IO - Pig + udfs - hadoop streaming

Learning on the data - difficult data - latest machine learning algorithms, not just existing mapreduce algorithms (mahout) - frameworks are starting to appear - Graphlab, or the Berkeley Spark ecosystem. - want to experiment on smaller data to reduce iteration time.

Prototype Learning Algorithm - loading text files into numpy arrays when memory constrained - JIT python compilation - scikit-learn - logistic regression - spectral clustering and the FEAST algorithm - nearest neighbors (output to gephi) - read/write binary formats

Implementation at scale - shoehorn into map-reduce - Port successful algorithms to GraphLab, C++ and MPI or Boost Graph Library etc. - MIT Starcluster .. - Numba, Blaze, Theano, KDT - Anaconda