---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=ZHpkLX2VFMU"'
Speakers: [Stefan Behnel]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/ZHpkLX2VFMU/hqdefault.jpg'
Title: '"The Cython Compiler for Python"'
date: '2014-07-22'
---
The Cython compiler is the most widely used static compiler for Python. The code it generates is used in countless critical applications that process huge amounts of data world wide. Cython has two major use cases: to compile Python code into fast native extension modules, and to connect native code to the CPython runtime. The main goal of the Cython project is to make it easy for users to manually optimise their Python code to make it run at C speed. This talk by one of the core developers will give an intro to using the compiler and an overview of its major features.

Outline will be more or less as follows:

*   Cython: intro to the project and the compiler (4 min.)
*   compiling Python code
    -   how to do it and what you get (3 min.)
    -   a tiny bit of distutils (2 min.)
*   static typing and Cython extensions to the Python language
    -   static typing in Cython language syntax (3 min.)
    -   static typing in pure Python syntax (2 min.)
    -   why Cython's type system is cool and what users need to know about it (8 min.)
    -   Cython for optimising Python code (5 min.)
*   quick intro: talking to native C/C++ code in Cython
    -   using external C APIs (4 min.)
    -   using external C++ APIs (3 min.)
    -   how to build and link in distutils (2 min.)
    -   notes on ways to wrap large C-APIs (1 min.)
*   quick overview: special features for high-performance code
    -   NumPy integration and memory views, fused types, parallel loops in all brevity (3 min.)
