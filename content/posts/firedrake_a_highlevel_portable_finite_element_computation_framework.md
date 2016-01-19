---
Category: 'EuroScipy 2014'
Copyright: 'youtube'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=VdzE0ZBAa-Q"'
Speakers: [Florian Rathgeber]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/VdzE0ZBAa-Q/hqdefault.jpg'
Title: '"Firedrake: a High-level Portable Finite Element Computation Framework"'
date: '2014-10-22'
---
In an ideal world, scientific applications are computationally efficient,
maintainable, composable and allow scientists to work very productively. In
this talk we demonstrate that these goals are achievable for a specific
application domain by choosing suitable domain-specific abstractions
implemented in Python that encapsulate domain knowledge with a high degree
of expressiveness.

We present [Firedrake](http://firedrakeproject.org/), a high-level Python framework for the portable
solution of partial differential equations on unstructured meshes with the
finite element method widely used in science and engineering. Firedrake is
built on top of [PyOP2](http://op2.github.io/PyOP2), a domain-specific language embedded in Python for
parallel mesh-based computations. Finite element local assembly operations
execute the same computational kernel for every element of the mesh and is
therefore efficiently parallelisable.

Firedrake allows scientists to describe variational forms and
discretisations for finite element problems symbolically in a notation very
close to the maths using the Unified Form Language [UFL](https://bitbucket.org/fenics-project/ufl/) from the [FEniCS project](http://fenicsproject.org/). Variational forms are translated into computational kernels by the
FEniCS Form Compiler [FFC](https://bitbucket.org/fenics-project/ffc/). Numerical linear algebra is delegated to PETSc,
leveraged via its petsc4py interface.

PyOP2 abstracts away the performance-portable parallel execution of these
kernels on a range of hardware architectures, targeting multi-core CPUs with
OpenMP and GPUs and accelerators with PyCUDA and PyOpenCL and distributed
parallel computations with mpi4py. Backend-specific code tailored to each
specific computation is generated, just-in-time compiled and efficiently
scheduled for parallel execution at runtime.

Due to the composability of the Firedrake and PyOP2 abstractions, optimised
implementations for different hardware architectures can be automatically
generated without any changes to a single high-level source. Performance
matches or exceeds what is realistically attainable by hand-written code.
Both projects are open source and developed at Imperial College London.
