---
Category: 'EuroScipy 2014'
Copyright: 'youtube'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=7rpcWZJaGFo"'
ThumbnailUrl: 'https://i.ytimg.com/vi/7rpcWZJaGFo/hqdefault.jpg'
date: '2014-10-22'
speakers: [Patrick Peglar]
tags: []
---
As scientific datasets continue to grow exponentially in size, the resource requirements of even simple analyses can quickly grow to become a problem -- e.g. the job takes an unreasonably long time, or simply runs out of space.

Existing solutions to this may be powerful, but can also come with a large complexity overhead, especially for the non-expert user. This makes adapting an existing analysis to the needs of larger datasets potentially very costly.

Biggus provides simple abstractions of data access and calculations which provide lazy evaluation. It exposes this as simple virtual array object which mimics a numpy array. Thus, it does not require the user to re-cast an operation in unfamiliar terms, or specify unrelated details of data storage or concurrency factors.

The lazy evaluation approach allows optimised resource usage for both storage accesses and the parallelisation of calculations. Pure Python is well suited to describing and implementing these techniques, and the resulting implementation is easily accessible to the average user.

At the Met Office, we develop data analysis tools for a large community of research scientists. We developed [Biggus](https://github.com/SciTools/biggus) as a resource for the Iris project, our next-generation analysis library for meteorological and oceanographic data (see: <http://scitools.org.uk/iris/>). While Biggus is still work-in-progress, within Iris it is already delivering significant benefit, in tasks such as catalogueing large datasets and accelerating statistical calculations. Here, performance already exceeds that of other standard software toolsets.

## Schedule

* the problems Biggus is aiming to solve, and techniques employed
* an overview of the architecture and code of the current implementation
* a demonstration of current performance, in ease-of-use and efficiency benefits
* suggestions for future developments; how to get involved; questions