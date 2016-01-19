---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/404_mrjob-distributed-computing-for-everyone.mp4
Speakers: [Jimmy Retzlaff]
Tags: [distributed, distributedcomputing, mrjob, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011MrjobDistributedComputingForEveryone940.png'
Title: '"mrjob: Distributed Computing for Everyone"'
date: '2011-03-11'
---
mrjob: Distributed Computing for Everyone

Presented by Jimmy Retzlaff

Have tons of data that needs analysis? Now it's as easy as 1-2-3! 1) Sign up
for an Amazon Web Services account. 2) Install Yelp's mrjob. 3) Write as few
as a dozen lines of Python code. This talk will show you how to use mrjob and
Amazon's Elastic MapReduce to easily process lots of data in parallel on a
potentially large cluster of computers that you can rent for a dime per
computer per hour.

Abstract

In their 2004 paper, Google outlined MapReduce - one of the programming models
they use to process large data sets. MapReduce is a relatively simple model to
develop for that allows the underlying framework to automatically parallelize
the job, add fault tolerance, and scale the job to many commodity computers.

In 2009, Amazon Web Services introduced their Elastic MapReduce (EMR) product.
It layers the Hadoop open source package on top of their Elastic Compute Cloud
(EC2) to allow anyone to rent a cluster of computers by the hour, starting at
about a dime per computer per hour, in order to run MapReduce jobs.

Some of the significant issues with Amazon's solution involve starting up
machine instances, replicating your code and its dependancies to EMR, running
and monitoring the job, and gathering the results.

So Yelp developed mrjob, which takes care of these details and lets the
developer focus on working with their data. Yelp uses mrjob to power many
internal jobs that work with its very large log files, for example:

  * People Who Viewed This Also Viewed... 
  * A user clicked an ad over and over, but we only want to charge the advertiser once 
  * We're thinking of a change, but want to simulate how that will affect ad revenue 

Now you can use that same power with just a few lines of Python.

Useful links:

  * Install mrjob: sudo easy_install mrjob 
  * Documentation: [http://packages.python.org/mrjob/](http://packages.python.org/mrjob/)
  * PyPI: [http://pypi.python.org/pypi/mrjob](http://pypi.python.org/pypi/mrjob)
  * Development is hosted at github: [http://github.com/Yelp/mrjob](http://github.com/Yelp/mrjob)

