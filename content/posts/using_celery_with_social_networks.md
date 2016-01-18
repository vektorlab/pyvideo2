---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=z751qhAzMb4"'
ThumbnailUrl: 'http://i.ytimg.com/vi/z751qhAzMb4/hqdefault.jpg'
date: '2012-09-05'
speakers: [David Gouldin]
tags: [celery, django]
---
Twitter conditionally rate limits based on IP address rather than access token
even when one is provided for some of its API calls. Facebook has at least 10
unique error messages to indicate a bad or expired access token (that I've
found so far). LinkedIn's pagination has an occasional off-by-one bug
resulting in an endless list of 1-user pages. Let's face it: interfacing with
social networks is tricky. Celery helps, but to provide stable, reliable, and
fast social features for your website, you'll need an arsenal of strategies
and tools to get you the rest of the way there.

By the end of this talk, you'll understand how to set up tasks to quickly
serve users with massive networks by employing intelligent distribution.
You'll be able to design robust processes to handle inconsistencies or
instabilities in 3rd party APIs. And you'll know how to have confidence that
the work you intend to do gets done, regardless of external rate limits,
pagination design, or API call dependency chains.

This talk is intended for people who have basic familiarity with celery and
would like to learn more about how to take advantage of it for large,
distributed task loads.

## Outline

I. Intro

A. 3rd party interfaces are hard

    
      * Speed
    
        * Much slower than local data
        * Users may still expect near-immediate results
    
      * Rate limits
    
        * Different rules for every service
        * Need to handle reactive & proactive as some don't publish rates
    
      * Instability
    
        * Outages (yes, Facebook does go down)
        * Random failures
    

B. Why Celery?

    
      * Asynchronous
      * Distributed
      * Fault tolerant
    

II. Task Organization

    
    A. Small, atomic tasks (1 API call per task)
    B. Minimal message state
    
       * Primitive types only (no model instances!)
       * Defer as much data access to the task itself as possible
    
    C. Create Task subclasses for common patterns
    D. Whenever possible, make tasks idempotent
    

III. Task Distribution

    
     A. Managing pagination
    
        * For a known set size
    
          * Where limit/offset is supported, launch all page tasks simlutaneously
          * Otherwise, 1 page launches the next as soon as the next cursor is obtained
    
        * For an unknown set size
    
          * Set max simultaneous pages
          * Task is terminal if blank, otherwise launches page w/ offset + max pages
    
        * Setting page size is an art, not a science
    
          * Minimize the number of api calls when possible
          * Avoid long-running tasks by setting a timeout ceiling
          * Avoid the temptation to pass API data to dependent tasks
    
     B. Tracking task dependencies ("Done?" is difficult for distributed systems)
    
        * Use an external backend to store a dependency tree
        * Subclass ResultSet to evaluate the task state of the tree
        * Requires ignore_result=False
    

IV. Rate Limiting

    
    A. Problems
    
       * Celery's rate limiting doesn't do what you think it does
       * 3rd party rate limits depend on many factors
    
    B. Solution
    
       * For services with known rate limits:
    
         * Use an external backend to store rate limit counters
         * Increment counters based on rate limit factors per api call
    
       * For services with unknown rate limits:
    
         * Use an external backend to store rate limit backoff counters
         * Ramp up / ratchet down call rate by power law as api calls fail/succeed
    

V. Failover

A. Problems

    
      * Celery's countdown doesn't do what you think it does
      * 3rd parties can fail in lots of "interesting" ways
    

B. Solution

    
      * Implement native RabbitMQ alternative to countdown
      * Create task base classes per social network to handle error conditions
    

VI. Multiple queues

    
    A. Better control over task priority management & resource distribution
    B. Not all social accounts are created equal (handling whales & spikes)
    C. When you can't stream updates, use a trickle queue
    

VII. Celerybeat considered harmful

    
     A. Periodic task persistence gets out of sync with code
     B. Just 1 more process to manage
     C. Cron: it's just. not. that. hard.
    

VIII. Debugging

    
      A. Don't use "always eager"
      B. Logging, logging, logging
      C. Unit tests are good, but integration tests save lives
    

IV. Gotchas

    
    A. Open socket prevents Celery soft timeout
    B. Celery soft timeout doesn't retry the task
    C. If result state is not known, Celery reports "PENDING"
    

