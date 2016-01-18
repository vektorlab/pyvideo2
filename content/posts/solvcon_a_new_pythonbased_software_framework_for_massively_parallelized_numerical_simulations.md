---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/382_solvcon-a-new-python-based-software-framework-for-massively-parallelized-numerical-simulations.mp4
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011SOLVCONANewPythonBasedSoftwareFrameworkForMass564.png'
date: '2011-03-11'
speakers: [Yung-Yu Chen]
tags: [gpgpu, numericalsimulations, parallelcomputing, pycon, pycon2011, simulations,
  solvcon]
---
SOLVCON: A New Python-Based Software Framework for Massively Parallelized
Numerical Simulations

Presented by Yung-Yu Chen

SOLVCON is the first Python-based software framework for high-resolution
simulations of multi-physics conservation laws. More than ninety percents of
the codes are done in Python. Performance hot-spots are optimized by C and
glued by ctypes library. SOLVCON is high-performance in nature and has been
able to utilize 512 4-core nodes at Ohio Supercomputer Center.

Abstract

In this decade, performance improvements of scientific computing will mainly
come from major changes in the computing hardware. A well-organized software
structure is imperative to accommodate such changes. Based on Python, SOLVCON
([http://solvcon.net/](http://solvcon.net/)) is designed as a software
framework to develop conservation-law solvers by segregating solving kernels
from various supportive functionalities. Being the governing equations for the
physical world, conservation laws are applied everywhere in science and
engineering. Although it is well known that the numerical algorithms and
physical models form the kernel of any conservation-law solver, few if not
none code can cleanly separate those core components from supportive
functionalities. The lack of organization has hindered the development of
legacy codes. To address the issues, the supportive functionalities are
internalized in the framework of SOLVCON. Aided by the framework, both multi-
physics and hybrid parallelism can be implemented in an organized way. To
date, SOLVCON has utilized up to 512 4-core nodes at Ohio Supercomputer Center
for high-resolution simulations of computational fluid dynamics (CFD). SOLVCON
targets to concurrently utilize thousands of computer nodes for high-
resolution simulations using over one billion mesh points.

One of the major purposes of SOLVCON is to resolve the complicated programming
efforts for GPU clusters. Supercomputing is undergoing the third revolution by
the emerging GPU computing. To date, the fastest supercomputer in the Top 500
list, Tianhe-1A, is a GPU cluster. GPU computing promises numerical analysts
to reduce the time for the high-resolution simulations from months to days. In
order to use GPU computing to accelerate such large-scale problems, GPU nodes
must be networked together to form a GPU cluster. As such, shared-memory and
distributed-memory parallelization must be simultaneously utilized to achieve
the so-called hybrid parallelism. Parallel computing is difficult, and hybrid
parallel computing is more difficult. By using Python to develop the
fundamental software structure, GPU or multi-threaded programming for shared-
memory parallelization are locked in solving kernels. Complex message-passing
is implemented in SOLVCON and isolated from solving-kernel developers. Highly
optimized C and GPU codes are glued into SOLVCON without loss of performance
by using the ctypes package. Othere important features of SOLVCON include:

  * Pluggable multi-physics.
  * Built-in [CESE](http://www.grc.nasa.gov/WWW/microbus/) solvers.
  * Unstructured mesh consisting of mixed elements.
  * Interface to Message-Passing Interface (MPI) libraries.
  * Socket communication layer: working without MPI installed.
  * Automatic distributed-memory parallelization by domain decomposition.
  * Parallel I/O.
  * In situ visualization by [VTK](http://vtk.org) library.
  * Standalone writers to VTK legacy and XML file formats.
  * Integration to supercomputer (cluster) batch systems.

SOLVCON has been applied to computation fluid dynamics and computational
mechanics. More physical solvers are being developed for various propagating
wave problems, e.g., electromagnetic waves. By using Python as the foundation
in SOLVCON, performance and extensibility are well balanced, and computational
research is being done in the most productive way. In this talk, the author of
SOLVCON will make an introduction to the software framework by including the
following topics:

  1. Simulations of conservation laws and hybrid parallelism for supercomputing.
  2. Issues in legacy codes and challenges to code for emerging supercomputer hardware.
  3. Using SOLVCON in the simple way by pre-defined modules.
  4. Fixed parts in SOLVCON. 
    1. Distributed computing.
    2. Multi-thread utilities.
  5. Customizable parts in SOLVCON. 
    1. Pluggable multi-physics and GPGPU computing.
    2. Supercomputer batch system and bootstrapping.
    3. In situ visualization.
  6. Conclusion.

The talk will take 30 minutes.

