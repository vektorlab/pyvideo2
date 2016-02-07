---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=F7NOKSP_vlQ'
Speakers: [Ian Ozsvald]
Tags: [cython, git, multiprocessing, network, numpy, nvidia, profiling, pycuda, runsnakerun,
  tutorial, windows, wxpython]
ThumbnailUrl: 'http://i.ytimg.com/vi/F7NOKSP_vlQ/hqdefault.jpg'
Title: 'Experiences making CPU-bound tasks run much faster'
date: '2011-07-18'
---
UPDATE - post-event I've created a [49 page PDF write-
up](http://ianozsvald.com/2011/06/29/high-performance-python-tutorial-v0-1
-from-my-4-hour-tutorial-at-europython-2011/) which summarises the 4 hour
tutorial

As a long-time R&D consultant I'm often working to make slow, experimental
code run faster for tasks like physics simulation, flood modeling and natural
language processing. Python allows a smooth progression from rough-and-ready
(but slow) algorithms through to finely tuned tasks that efficiently use as
much CPU power as you can bring to bear. Speed-ups of 10-500* can be expected
for the Mandelbrot code we'll use.

In this talk I'll cover a set of libraries that make CPU-bound tasks run much
faster. We'll begin with a look at profiling using RunSnakeRun and
line_profiler to identify our bottleneck. We'll take a look at slow algorithms
in Python and how they can run faster using numpy and numexpr.

Next we'll cover the use of multiprocessing to utilise multiple CPU cores
along with Cython or ShedSkin to easily use C code in a friendly Python
wrapper. Multiprocessing on a quad-core system can often provide a 4* speed-up
for the right tasks. Next parallelpython will let us run our code on a network
of machines.

Finally we'll look at pyCUDA to utilise an NVIDIA GPU. CUDA can give the best
improvements for mathematical problems (over 100* on the right tasks) but
works on a narrower set of problems.

How it'll work: The tutorial will be hands on, you'll be converting example
files from normal Python to faster variants using the tools below. All of it
is optional, you'll get the most benefit by having everything installed. We'll
work in groups and open discussion is encouraged.

NOTE - you are expected to have all these tools installed _before_ the
tutorial (if you don't, you might find it hard to follow what's going on!).

I'll be using Python 2.7.1 on a Macbook (Snow Leopard). All of these tools run
on Windows and Linux, as long as your versions are fairly recent everything
should run just fine.

My versions (roughly ordered by importance):

  * Python 2.7.1
  * RunSnakeRun 2.0.1b6 (with wxPython 2.8.12.0 Unicode)
  * line_profiler (1.0b2)
  * Cython 0.14.1
  * ShedSkin 0.7.1
  * numpy 1.5.1
  * numexpr 1.4.2
  * ParallelPython 1.6.1
  * pyCUDA HEAD from git as of 14th June 2011 (with CUDA 4.0 drivers)
  * PyPy 1.5

Some background reading:

  * [http://ianozsvald.com/2010/07/14/22937-faster-python-math-using-pycuda/](http://ianozsvald.com/2010/07/14/22937-faster-python-math-using-pycuda/)
  * [http://ianozsvald.com/2008/11/17/making-python-math-196-faster-with-shedskin/](http://ianozsvald.com/2008/11/17/making-python-math-196-faster-with-shedskin/)

