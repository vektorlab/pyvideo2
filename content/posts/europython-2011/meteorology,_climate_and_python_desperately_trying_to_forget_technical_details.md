---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=zZY-5cHZsT0'
Speakers: [Claude Gibert]
Tags: [framework, nasa, parallel, performance, 'python,', scientific]
ThumbnailUrl: 'http://i.ytimg.com/vi/zZY-5cHZsT0/hqdefault.jpg'
Title: 'Meteorology, Climate and Python: desperately trying to forget technical details'
date: '2011-07-13'
---
# Contents

Python is a great language for writing programming frameworks. Python
frameworks are normally addressed to software developers who are Python
professionals. I developed a software package in a scientific institution,
designed to be used by non-programmers, but also designed to enable
customisation through programming by some users. I finally designed a three
level package:

  * A Python programming framework, addressed whoever wanted to invest in Python and had plans to develop applications;

  * An application built on that framework with an interface designed for non-programmers;

  * Ways of customising the behaviour of the application by providing some basic Python functions or more elaborated code.

One of the challenges was to offer an application with an easy to use
interface, not graphical, not web-based and not requiring Python programming.
This interface was necessary for batch processing.

This talk addresses how this project was carried out, the technical solutions
adopted and how Python was introduced in an operational scientific institution
([http://www.ecmwf.int](http://www.ecmwf.int)) where most users were Fortran
programmers. Python was introduced as early as 2004 and it was a challenge to
gain acceptance. I will also make a parallel with a project I am currently
working on for NASA
([http://gmao.gsfc.nasa.gov/](http://gmao.gsfc.nasa.gov/)). _Desperately
trying to forget technical details_ summarises how I tried, using Python, to
help Meteorology scientists to focus on their domain of expertise instead of
constantly solving technical problems.

# Background:

The disciplines of Meteorology and Climate involve numerical modelling of
physical phenomena. The amount of data going in and out of the model is
considerable. The organisation and the storage of data is complicated, their
post-processing is a challenge. Scientists need to access and process input
and output data to monitor the trends of the input data and to evaluate the
performance of their models. Those statistics, diagnostics, plots and
verifications are crucial to the improvement of the quality of the models.
Finding the right data, decoding it, transforming it to be ready for use are
necessary steps to initiate the pre-processing. All these actions are
fundamentally the same between different prediction centres, but the data
organisation and file formats can differ.
