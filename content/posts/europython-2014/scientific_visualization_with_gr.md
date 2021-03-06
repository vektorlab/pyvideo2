---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=-oSAMkqbWjs'
Speakers: [Josef]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/-oSAMkqbWjs/hqdefault.jpg'
Title: 'Scientific Visualization with GR'
date: '2014-07-25'
---
Python has long been established in software development departments of research and industry, not least because of the proliferation of libraries such as *SciPy* and *Matplotlib*. However, when processing large amounts of data, in particular in combination with GUI toolkits (*Qt*) or three-dimensional visualizations (*OpenGL*), it seems that Python as an interpretative programming language may be reaching its limits.

---

*Outline*

- Introduction (1 min)
    - motivation
- GR framework (2 mins)
    - layer structure
    - output devices and capabilities
- GR3 framework (1 min)
    - layer structure
    - output capabilities (3 mins)
        - high-resolution images
        - POV-Ray scenes
        - OpenGL drawables
        - HTML5 / WebGL
- Simple 2D / 3D examples (2 min)
- Interoperability (PyQt/PySide, 3 min)
- How to speed up Python scripts (4 mins)
    - Numpy
    - Numba (Pro) 
- Animated visualization examples (live demos, 6 mins)
    - physics simulations
    - surfaces / meshes
    - molecule viewer
    - MRI voxel data
- Outlook (1 min)

*Notes*

Links to similar talks, tutorials or presentations can be found [here][1]. Unfortunately, most of them are in German language.

The GR framework has already been presented in a talk at PyCon DE [2012][2] and [2013][3], during a [poster session][4] at PyCon US 2013, and at [PythonCamps 2013][5] in Cologne. The slides for the PyCon.DE 2013 talk can be found [here][6].

As part of a collaboration the GR framework has been integrated into [NICOS][7] (a network-based control system completely written in Python) as a replacement for PyQwt.

  [1]: http://gr-framework.org/
  [2]: https://2012.de.pycon.org/programm/schedule/sessions/54
  [3]: https://2013.de.pycon.org/schedule/sessions/45/
  [4]: https://us.pycon.org/2013/schedule/presentation/158/
  [5]: http://josefheinen.de/rasberry-pi.html
  [6]: http://iffwww.iff.kfa-juelich.de/pub/doc/PyCon_DE_2013
  [7]: http://cdn.frm2.tum.de/fileadmin/stuff/services/ITServices/nicos-2.0/dirhtml/
