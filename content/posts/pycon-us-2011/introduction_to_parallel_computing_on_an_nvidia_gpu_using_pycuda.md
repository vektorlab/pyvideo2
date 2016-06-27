---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/436_introduction-to-parallel-computing-on-an-nvidia-gpu-using-pycuda.mp4
Speakers: [Roy Hyunjin Han]
Tags: [nvidia, parallel, pycon, pycon2011, pycuda]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011IntroductionToParallelComputingOnAnNVIDIAGPUU724.png'
Title: 'Introduction to Parallel Computing on an NVIDIA GPU using PyCUDA'
date: '2011-03-11'
---
Introduction to Parallel Computing on an NVIDIA GPU using PyCUDA

Presented by Roy Hyunjin Han

With Andreas Klöckner's PyCUDA, you can harness the massively parallel
supercomputing power of your NVIDIA graphics card to crunch numerically
intensive scientific computing applications in a fraction of the runtime it
would take on a CPU and at a fraction of the development cost of C++. We'll
cover hardware architecture, API fundamentals and several examples to get you
started.

Abstract

There are two approaches to parallelizing a computationally heavy procedure:
use a messaging queue such as AMQP to distribute tasks among a networked
cluster or increase the number of processors in a single machine. This talk
focuses on techniques for adapting mathematical code to run on specialized
multi-core graphic processors.

Modern graphic processors have hard-coded transistors for common vector and
matrix operations, making them ideal for general scientific computing.
However, the NVIDIA CUDA's unique design requires knowledge of its hardware to
adapt algorithms effectively. This talk covers basic CUDA architecture, API
functions and several examples to illustrate the different kinds of problems
that will benefit from parallelization.
