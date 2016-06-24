---
Category: 'EuroScipy 2014'
Copyright: 'youtube'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=QSlo_Nyzeig'
Speakers: [Giannis Ashiotis, Jerome Kieffer]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/QSlo_Nyzeig/hqdefault.jpg'
Title: 'PyFAI: a Python library for high performance azimuthal integration on GPU'
date: '2014-10-22'
---
In the field of X-Ray diffraction, 2D area detectors like ccd or pixel detectors have become popular in the last 15 years for diffraction experiments thanks to the large solid-angle coverage and to their better signal linearity. These detectors have a large sensitive area of millions of pixels with high spatial resolution and are getting fast: one kilo-Hertz is expected this year. The software package pyFAI we present here has been designed to reduce X-ray 2D-diffraction images into 1D curves (azimuthal integration) usable by other software for in-depth analysis such as Rietveld refinement, ... Other averaging patterns like 2D integration, image distortion, ... are also available. PyFAI is a library featuring a clean pythonic interface and aiming at being integrated into other software. But it also needs to cope with the data deluge coming from the detector...

In this contribution, we would like to highlight the performance reached by this library. To get today’s computers best performances, one needs to have parallelized code and azimuthal integration is not directly parallelizable. After a scatter-to-gather transformation of the algorithm, it got parallel (Cython implementation). Other optimizations have been used to get the best performances out of GPU (compensated summation, partial parallel reductions, ...). 