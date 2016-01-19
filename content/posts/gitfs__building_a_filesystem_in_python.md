---
Category: 'PyCon Italia 2015'
Copyright: ''
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=elA96lMW-gA"'
Speakers: [Emanuel Danci, Vlad Temian]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/elA96lMW-gA/maxresdefault.jpg'
Title: '"gitfs - building a filesystem in Python"'
date: '2015-05-29'
---
gitfs is an open-source[1] filesystem which was designed to bring the full powers of Git to everyone, no matter how little they know about versioning. A user can mount any repository and all the his changes will be automatically converted into commits. gitfs will also expose the history of the branch you’re currently working on by simulating snapshots of every commit.
gitfs is useful in places where you want to keep track of all your files, but at the same time you don’t have the possibility of organizing everything into commits yourself. A FUSE filesystem for git repositories, with local cache.
In this talk we will take a look at some of the crucial aspects involved in building a reliable FUSE filesystem, the steps that we took in building gitfs,  especially in handling the git objects (http://git-scm.com/book/en/v2/Git-Internals-Git-Objects), what testing methods we have used for it and also we will share the most important lessons learned while building it. 
The prerequisites for this talk are:

A good understanding of how Git works
Basic understaning of Operating Systems concepts 

[1] You can get the source here - https://github.com/PressLabs/gitfs; you cand find more details here -  http://www.presslabs.com/gitfs/.
