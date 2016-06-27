---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/409_packaging-from-distutils-to-distutils2.mp4
Speakers: []
Tags: [distutils, distutils2, pycon, pycon2011, setup.py, setuptools, zc.buildout]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011PackagingFromDistutilsToDistutils2901.png'
Title: 'Packaging, from Distutils to Distutils2'
date: '2011-03-11'
---
Packaging, from Distutils to Distutils2

Tarek Ziadé

Packaging or installing a Python application can be extremely painful. This
talk will deep-dive into the new Distutils2 features and explain how you can
use them in your project *today* to make life easier for everyone (users, OS
package managers, developers, etc.).

Abstract

  1. Distutils2 presentation and goals 
    1. Framework 
    2. Command-driven packaging system 
    3. Changes from Distutils1 
      1. R.I.P. setup.py 
      2. The new metadata fields (PEP 345) 
      3. versions for your project (PEP 386) 
      4. PyPI goodies 
        1. browsing 
        2. uploading docs 
      5. What's installed ? what to install ? (PEP 376) 
        1. The Dependency graph tool 
      6. Extensibility ! 
        1. commands 
        2. compilers 
    4. Pysetup, one command to rule them all 
      1. install ! 
      2. remove 
      3. do other things 
    5. Examples 
      1. Example 1: A simple Distutils2 project 
      2. Example 2: Porting your project to Distutils2, and keep it working in Distutils/Setuptools/zc.buildout environments. 
      3. Example 3: Creating and releasing your own commands and compilers 
      4. Example 4: Developement process made simple with Distutils2 
    6. Conclusion 
      1. Roadmap 
