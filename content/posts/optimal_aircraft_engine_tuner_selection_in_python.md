---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/380_optimal-aircraft-engine-tuner-selection-in-python.mp4
Speakers: [Jeffrey Armstrong]
Tags: [aircraftenginetuning, casestudy, pycon, pycon2011, scipy]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011OptimalAircraftEngineTunerSelectionInPython133-714.jpg'
Title: '"Optimal Aircraft Engine Tuner Selection in Python"'
date: '2011-03-11'
---
Optimal Aircraft Engine Tuner Selection in Python

Presented by Jeffrey Armstrong

A numerical algorithm for designing on-board aircraft engine diagnostics has
been implemented in Python. Employing the optimization techniques within
SciPy, the code performs a search for an optimal vector of parameters for
estimating engine variables, including exhaust temperatures and thrust. The
algorithm exploits the numerical strengths of Python and SciPy for speed and
interoperability.

Abstract

An emerging field of aircraft engine diagnostics is the inclusion of on-board
engine performance tracking algorithms. These algorithms utilize data provided
by a limited number of engine sensors to determine the current engine
performance, which tends to degrade over time. However, estimating engine
performance instantaneously is problematic due to the limited number of
sensors normally available on a commercial aircraft engine.

One common practice is to estimate and track engine performance in software
using a Kalman filter, a mathematical construct for tuning a numerical model
to better track actual measurements (1). A new technique has been devised to
optimize the design of this filter in aircraft engine applications (2). An
optimization procedure to aid in the design of the filter has been implemented
in Python and exercised against the significant number of minimization and
optimization strategies available in SciPy. The talk focuses on the design of
this optimization procedure in Python. The object-oriented nature of Python
offers benefits over alternative numerical languages; speed, availability, and
maintainability played central roles in the selection of Python as the
implementation language. The availability of the multiprocessing module
allowed for full utilization of modern multi-core CPUs, in contrast with often
limited commercial numerical computing packages, further improving
computational speed.

Some difficulties were encountered during this design exercise. Discussion of
these obstacles and their eventual solution is presented. Specifically,
iterative solvers for the discrete algebraic Riccati equation and the discrete
Lyapunov equation had to be authored in Python (3,4). Additional framework for
working with discrete state-space control systems was created, exploiting the
object-oriented features of the language (5).

The Python implementation was able to verify the solution of the optimization
problem. Comparison with an alternative, reference MATLAB implementation will
be presented briefly. The results of this research is planned to be presented
at the American Society for Mechanical Engineers Turbo Expo 2011 Conference in
June, 2011 (6). The algorithm design in Python is meant to showcase the
ability to perform controls engineering tasks in the Python language
efficiently.

1. “Kalman Filter,” Wikipedia: [http://en.wikipedia.org/wiki/Kalman_filter](ht
tp://en.wikipedia.org/wiki/Kalman_filter)

2. Simon, D. L. and Garg, S., “Optimal Tuner Selection for Kalman Filter-Based
Aircraft Engine Performance Estimation”. Journal of Engineering for Gas
Turbines and Power. March 2010, Vol. 132.

3. “Algebraic Riccati Equation,” Wikipedia: [http://en.wikipedia.org/wiki/Alge
braic_Riccati_equation](http://en.wikipedia.org/wiki/Algebraic_Riccati_equatio
n)

4. “Lyapunov Equation,” Wikipedia: [http://en.wikipedia.org/wiki/Lyapunov_equa
tion](http://en.wikipedia.org/wiki/Lyapunov_equation)

5. “State Space,” Wikipedia: [http://en.wikipedia.org/wiki/State-
space](http://en.wikipedia.org/wiki/State-space)

6. Simon, D. L., Armstrong, J. B., "Application of an Optimal Tuner Selection
Approach for On-Board Self-Tuning Engine Models," Proceedings of the ASME
Turbo Expo 2011, GT2011-46408, 2011 (To Be Published).

