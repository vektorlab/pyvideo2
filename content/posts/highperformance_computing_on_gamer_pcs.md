---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=TkBkGGPY2P0"'
ThumbnailUrl: 'http://i.ytimg.com/vi/TkBkGGPY2P0/hqdefault.jpg'
date: '2011-07-13'
speakers: [Yann Le Du]
tags: [image, mapping, nvidia, performance, processing, science, scientific]
---
In Electron Paramagnetic Resonance Imaging, we are faced with a deconvolution
problem that has a strong impact on the image actually reconstructed. Faced
with the need of mapping the distribution of organic matter in Terrestrial and
Martian rock samples for applications in exobiology, we needed to see how to
extract a maximum amount of information from our data: our approach uses
reservoir computing artificial neural networks coupled to a particle swarm
algorithm that evolves the reservoirs’ weights.

The code runs on the Hybrid Processing Units for Science (HPU4Science) cluster
located at the Laboratoire de Chimie de la Matière Condensée de Paris (LCMCP).
The cluster is composed of a central data storage machine and a heterogeneous
ensemble of 6 decentralized nodes. Each node is equipped with a Core2 Quad or
i7 CPU and 3-7 NVIDIA Graphical Processing Units (GPUs) including the GF110
series. Each of the 28 GPUs independently explores a different parameter space
sphere of the same problem. Our application shows a sustained real performance
of 15.6 TFLOPS. The HPU4Science cluster cost $36,090 resulting in a 432.3
MFLOPS/$ cost performance.

That talk is meant to demonstrate on a practical case how consumer grade
computer hardware coupled to a very popular computer language can be used to
tackle a difficult yet very elementary scientific problem: how do you go from
formulating the problem, to choosing the right hardware and software, and all
the way to programming the algorithms using the appropriate development tools
and methodologies (notably Literate Programming). On the math side, the talk
requires a basic understanding of matrix algebra and of the discretization
process involved when computing integrals.

