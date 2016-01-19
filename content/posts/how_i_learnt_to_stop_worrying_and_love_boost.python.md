---
Category: 'PyCon ZA 2015'
Copyright: ''
Language: 'English'
SourceUrl: '"http://youtu.be/2urUj9NRqFc"'
Speakers: [Bruce Merry]
Tags: [Room 215]
ThumbnailUrl: 'https://i.ytimg.com/vi/2urUj9NRqFc/hqdefault.jpg'
Title: '"How I learnt to stop worrying and love Boost.Python"'
date: '2015-10-02'
---
The Zen of Python dictates that there should be one - and preferably only one - obvious way to do something. However, when it comes to interoperation with C and C++, there is a multitude of options: the Python C API, Boost.Python, ctypes, cffi, Cython. I will describe my quest to find the **holy grail**^W^W **right interface** for a high-performance networking library.

The talk is largely a case study in applying Boost.Python, and will look at some issues such as the Global Interpreter Lock, handling KeyboardInterrupt cleanly, and managing object lifetime. I will briefly mention some of the alternative tools to explain why I settled on Boost.Python. It is not a complete Boost.Python tutorial, but rather aims to give a sense of the flavour and show how it's used in a real application.

For obvious reasons, this talk will have a lot of C++ code in it, and some familiarity with C++ will be useful.