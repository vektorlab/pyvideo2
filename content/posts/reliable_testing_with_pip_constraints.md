---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=aZ_y_U6rZRM"'
Speakers: [Robert Collins]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/aZ_y_U6rZRM/hqdefault.jpg'
Title: '"reliable testing with pip constraints"'
date: '2015-08-04'
---
pip freeze files and similar techniques like buildout have been used for reliable testing and reliable deployments for some time. But they are not flexible enough to deal with situations like OpenStack where there are dozens of separate codebases, evolving independently, which still need the same rigour and reliability.

Enter pip constraints, new in 7.1.0. I will cover their use, design, and how we're using them in devstack (and thus OpenStack CI) - and how you can (and should) use them in your local projects.

