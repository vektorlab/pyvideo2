---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=Iw0MwPL2FCU'
Speakers: [Jim Baker]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/Iw0MwPL2FCU/hqdefault.jpg'
Title: 'Scalable Realtime Architectures in Python'
date: '2014-07-25'
---
Increasingly we are interested in implementing highly scalable and
fault tolerant realtime architectures such as the following:

* Realtime aggregation. This is the realtime analogue of working with
  batched map-reduce in systems like Hadoop.

* Realtime dashboards. Continuously updated views on all your
  customers, systems, and the like, without breaking a sweat.

* Realtime decision making. Given a set of input streams, policy on
  what you like to do, and models learned by machine learning, optimize a
  business process. One example includes autoscaling a set of servers.

(We use realtime in the soft sense: systems that are continuously
computing on input streams of data and make a best effort to keep up;
it certainly does not imply hard realtime systems that strictly
bound their computation times.)

Obvious tooling for such implementations include Storm (for event
processing), Kafka (for queueing), and ZooKeeper (for tracking and
configuration). Such components, written respectively in Clojure
(Storm), Scala (Kafka), and Java (ZooKeeper), provide the desired
scalability and reliability. But what may not be so obvious at first
glance is that we can work with other languages, including Python, for
the application level of such architectures. (If so inclined, you can
also try reimplementing such components in Python, but why not use
something that's been proven to be robust?)

In fact Python is likely a better language for the app level, given
that it is concise, high level, dynamically typed, and has great
libraries. Not to mention fun to write code in! This is especially
true when we consider the types of tasks we need to write: they are
very much like the data transformations and analyses we would have
written of say a standard Unix pipeline. And no one is going to argue
that writing such a filter in say Java is fun, concise, or even
considerably faster in running time.

So let's look at how you might solve such larger problems. Given that
it was straightforward to solve a small problem, we might approach as
follows. Simply divide up larger problems in small one. For example,
perhaps work with one customer at a time. And if failure is an ever
present reality, then simply ensure your code retries, just like you
might have re-run your pipeline against some input files.

Unfortunately both require distributed coordination at scale. And
distributed coordination is challenging, especially for real systems,
that will break at scale. Just putting a box in your architecture
labeled **"ZooKeeper"** doesn't magically solve things, even if
ZooKeeper can be a very helpful part of an actual solution.

Enter the Storm framework. While Storm certainly doesn't solve all
problems in this space, it can support many different types of
realtime architectures and works well with Python. In particular,
Storm solves two key problems for you.

**Partitioning**. Storm lets you partition streams, so you can break
down the size of your problem. But if the a node running your code
fails, Storm will restart it. Storm also ensures such topology
invariants as the number of nodes (spouts and bolts in Storm's lingo)
that are running, making it very easy to recover from such failures.

This is where the cleverness really begins. What can you do if you can
ensure that **all the data** you need for a given continuously updated
computation - what is the state of this customer's account?  - can be
put in **exactly one place**, then flow the supporting data through it
over time? We will look at how you can readily use such locality in
your own Python code.

**Retries**. Storm tracks success and failure of events being
processed efficiently through a batching scheme and other
cleverness. Your code can then choose to retry as necessary. Although
Storm also supports exactly-once event processing semantics, we will
focus on the simpler model of at-least-once semantics. This means your
code must tolerate retry, or in a word, is idempotent. But this is
straightforward. We have often written code like the following:

    seen = set()
    for record in stream:
        k = uniquifier(record)
        if k not in seen:
           seen.add(k)
           process(record)

Except of course that any such real usage has to ensure it doesn't
attempt to store all observations (first, download the Internet! ;),
but removes them by implementing some sort of window or uses data
structures like HyperLogLog, as we will discuss.

One more aspect of reliability we will discuss is how to compose
reliable systems out of reliable components; we will show how this
can be readily done with a real example of consuming Kafka and
tracking consumption progress in ZooKeeper.
