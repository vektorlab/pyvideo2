---
Category: 'Kiwi PyCon 2015'
Copyright: 'CC BY-SA'
Language: 'English'
SourceUrl: 'http://youtu.be/L-FyCT02gqc'
Speakers: [Chris LeBlanc]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/L-FyCT02gqc/hqdefault.jpg'
Title: 'Cython: get the benefits of C without leaving Python'
date: '2015-09-05'
---
Cython is an optimising static compiler based on Pyrex, created by Greg Ewing from the university of Canterbury.  It bridges the worlds of Python and C, letting you write code that runs close to C speed in a syntax that is very close to Python.  This talk will show how you can speed up a typical Python program with Cython datatypes.  We’ll call C functions directly, passing NumPy arrays with ease.  We’ll see how we can release the global interpreter lock, letting us run multiple threads in parallel near C speeds.  We’ll look at Cython’s parallel module for data parallelism and compare it to some alternatives and discuss the pros and cons.