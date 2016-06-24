---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=MoL2nDYcW1U'
Speakers: [Giovanni Bajo]
Tags: [matplotlib, py2exe, pyqt]
ThumbnailUrl: 'http://i.ytimg.com/vi/MoL2nDYcW1U/hqdefault.jpg'
Title: 'Distributing Python programs through PyInstaller'
date: '2011-07-20'
---
The talk will focus on how to distribute multi-platform proprietary Python
applications, using [PyInstaller](http://www.pyinstaller.org).

PyInstaller takes a program written in Python and turns it into a static
executable (binary) that does not depend upon an existing Python installation,
nor third party library. The executable can then be packed and shipped in many
different ways (through installer wizards, deb/rpm packages, etc.).

PyInstaller is a good multi-platform alternative to tools like py2exe and
py2app, but it found troubles to gain acceptance in a market that seems
strongly tied to older tools. Instead, PyInstaller puts forward important new
features: for instance, it works on the most important desktop platforms
(Windows, Linux/UNIX, Mac), and it has got an automatic and fully transparent
support for all the workarounds needed to make applications using complex
libraries like Matplotlib or PyQt work within a static executable.

In detail, the following points will be discussed:

  * Distribution of a priopriertary software: initial requests
  * PyInstaller: how it works (basic tutorial)
  * The secrets of PyInstaller: technical details
  * Import hooks: effectively handling third party extensions
  * Flexibility with PyInstaller: what goes in and what stays out
  * Linux: static binaries for a single distribution or cross-distributions
  * Mac: creation of bundles for graphic applications

