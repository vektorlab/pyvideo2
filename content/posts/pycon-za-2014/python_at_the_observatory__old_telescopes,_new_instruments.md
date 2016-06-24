---
Category: 'PyCon ZA 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://archive.org/details/pyconza2014-python-at-the-observatory'
Speakers: [Carel van Gend; Briehan Lombaard]
Tags: [pyconza, pyconza2014]
ThumbnailUrl: 'http://archive.org/download/pyconza2014-python-at-the-observatory/pyconza2014-python-at-the-observatory.thumbs/15%20Python%20at%20the%20Observatory%20-_002130.jpg'
Title: 'Python at the Observatory - Old telescopes, new instruments'
date: '2014-10-03'
---
Astronomy in South Africa has a long and illustrious history. In addition to the premier, 10-m Southern Africa Large Telescope (SALT) , there are a number of small- and medium-sized telescopes hosted at the South African Astronomical Observatory that still produce a great deal of valuable data. We'd like to show how we're using new instruments and the nimbleness of Python to bring seventy-year-old telescopes into the 21st century.
Our long-term goal is to have the telescopes and associated instruments be remotely operable, easy to use, and robust enough that valuable data is reliably captured and stored. In addition, we want to make it as easy as possible to update and improve the software which controls the instruments.
We have developed a distributed framework to control the instruments. Drivers for individual components may be written in whichever language is most suitable (we've used C, C++ and Python where appropriate). These drivers communicate over a TCP/IP socket with a Python controller process, and on top of that is a Python/Flask driven web interface.
We plan to adapt the framework to new instruments (such as a wide-field camera for the 1.9- and 1-m telescopes), under-development instruments (such as an upgrade to the Cassegrain spectrograph on the 1.9-m telescope), and retrofit to older instruments as feasible.
As a demonstration of the new framework, we will present our work of migrating the control software for the Sutherland High-speed Optical Camera (SHOC) from being a disparate collection of proprietary, Windows-based software, to a unified, open, web accessible system. SHOC is a high-speed, accurately-timed, imaging instrument that can be mounted on the 1.9-, 1-, and 0.75-m telescopes in Sutherland, control of which includes that for a camera, a global positioning system (GPS), and a filter wheel.