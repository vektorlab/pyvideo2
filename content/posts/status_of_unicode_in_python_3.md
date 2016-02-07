---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/364_status-of-unicode-in-python-3.m4v
Speakers: [Victor Stinner]
Tags: [pycon, pycon2011, python3, unicode]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011StatusOfUnicodeInPython3393.png'
Title: 'Status of Unicode in Python 3'
date: '2011-03-11'
---
The talk will focus on the recent issues fixed in Python 3.1 and 3.2:

  * Use the PEP 383 (error handler to store undecodable bytes) everywhere 
  * Encoding of the command line arguments: utf-8 on Mac OS X, locale encoding on UNIX/BSD, unicode on Windows 
  * Environment variables: creation of os.environb 
  * Filenames: huge work to support the PEP 383 everywhere, creation of os.fsencode() and os.fsdecode() 
  * Python source code encoding: use tokenize.detect_encoding() instead of the locale encoding 
  * some library examples: email, ftp, ... 
  * etc. 

The talk will present not only the changes in Python, but also in the C API.

