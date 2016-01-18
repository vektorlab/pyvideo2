---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/450_supercomputer-and-cluster-application-performance-analysis-using-python.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011SupercomputerAndClusterApplicationPerformanceAna648.png'
date: '2011-03-11'
speakers: [Daniel W. Barnette]
tags: [pycon, pycon2011, pylot, sandianationallaboratories, supercomputer]
---
PyCon 2011: Supercomputer and Cluster Application Performance Analysis using
Python

Presented by Daniel W. Barnette, PhD

Sandia National Labs analyzes high-performance computing environments to
optimize application performance, analyze system architectures, and provide
design guidance for future systems. We discuss 1) generating performance data
across multiple systems using mini-applications, and 2) using our open source
Python tools Pylot/Co-Pylot to store and analyze data using a MySQL database
server.

Abstract

Sandia National Laboratories analyzes large-scale, state-of-the-art high
performance computing environments for the Department of Energy (DOE),
Department of Defense (DoD), and other government agencies. Execution
efficiency is vital when dealing with datasets that require billions of
elements or when running simulations that take millions of core-hours to
complete.

One approach to investigating execution efficiency is to instrument our large-
scale applications and platforms to generate timings and other performance
data. Although effective in mature computing environments, working directly
with large-scale applications is cumbersome, time consuming, and even
impossible in the early stages of computer system analysis and design.
Furthermore, the software and data sets of these applications may be
restricted, limiting our abilities to collaborate.

In order to enhance our analysis capabilities far upstream from when large-
scale applications can be used and when working with external collaborators,
we have developed a collection of mini-applications that capture the essence
of our much larger scientific codes, are readily applicable to both large and
small systems, and whose run-time information can accurately reveal problems
associated with execution efficiency.

Generating the data is only half the problem, though. We need the ability to
capture platform-relevant mini-app performance data at the convenience of the
testers when and where they generate the data. We also need the ability to
search through, filter, and visualize the resulting performance measurement
datasets in detail to identify and understand trends and patterns.

Sandia National Laboratories has developed a performance analysis suite
primarily consisting of two tools written in Python, Pylot and Co-Pylot. Co-
Pylot is a relatively simple interface that enables easy batch transfer of
performance data to a remote MySQL database server for persistent storage.

Once stored, the performance data is extracted, organized, filtered, and
analyzed using Pylot, a more functionally complex interface. Pylot is used to
present user-selected MySQL database fields in a variety of views including
statistical data, bar and pie charts, Cartesian or log-log or semi-log plots,
reference curves for comparisons, and Kiviat diagrams (also called radar
charts) for multivariate datasets.

A built-in storage buffer provides the ability to store, compare, and analyze
data from multiple databases. This capability is critical for studying
performance variations of a code running on a particular architecture,
comparing application performance across architectures, or comparing multiple
applications on one or more architectures. Values in up to four database
fields at a time can be mathematically combined to generate a new temporary
field to provide complete generality while accessing a database. Further,
Pylot provides the ability to easily move MySQL databases and tables between
computers, including the analyst’s laptop. This coherency of databases across
multiple analysis platforms can be used, for example, to avoid network latency
issues associated with accessing remote servers. It also serves as a
distributed backup system.

An outline of this presentation follows:

  1. Applications at Sandia National Laboratories (6 mins) 
    * Simulation size and runtime of typical large Sandia applications 
    * Difficulties of using large-scale applications in early computer system design and analysis 
    * Mantevo mini-apps – small, self-contained programs that embody essential performance characteristics of key applications. 
  2. Gathering data (4 mins) 
    * What information Mantevo mini-apps provide 
    * Co-Pylot – getting your data into a remote database 
  3. Supercomputer and Cluster application analysis (10 mins) 
    * Pylot – demo of accessing and graphing MySQL data as a method for analyzing performance 
    * Diagnosing performance issues 
    * Comparing different systems and different runs 
  4. Future Extensions of Pylot (5 mins) 
    * Capturing compile-time and execution info 
    * Efforts to move parts of Pylot to the web 

