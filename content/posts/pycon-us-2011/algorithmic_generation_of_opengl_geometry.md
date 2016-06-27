---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/381_algorithmic-generation-of-opengl-geometry.mp4
Speakers: [Jonathan Hartley]
Tags: [3d, opengl, pycon, pycon2011, pyglet, pyopengl]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011AlgorithmicGenerationOfOpenGLGeometry275-566.jpg'
Title: 'Algorithmic Generation of OpenGL Geometry'
date: '2011-03-11'
---
Algorithmic Generation of OpenGL Geometry

Presented by Jonathan Hartley

Starting from a basic 'hello world' OpenGL app, a simple and Pythonic model of
3D polyhedra is presented, with neat generators to convert these into ctype
arrays for OpenGL. Geometric algorithms then generate some fun geometry, and
these are compounded to produce successively more complex and interesting
shapes.

Abstract

The author's intent is to demonstrate that effective stylistic 3D graphics can
be achieved using surprisingly small amounts of code. This hopefully makes the
topic amenable to 3D beginners, while possibly suggesting some alternative
approaches to those with 3D experience.

Talk Outline

Throughout, discussion of ideas and code dissection alternates with live
animated demos, at 60fps on very modest hardware.

  1. Inspirations - Effective non-photo-realistic work in gaming, movies and the demo scene. (1m) 
  2. A convenient & Pythonic way to model 3D polyhedra, and some neat generators to convert these into OpenGL arrays at runtime. (7m) 
  3. Composition of polyhedra to create more complex shapes. (3m) 
  4. The resulting performance characteristics: What works well from Python, and what doesn't. (2m) 
  5. Koch tetrahedron & tetrix, aka Sierpinski tetrahedron. (1m) 
  6. Surprisingly effective 3D models created from small bitmaps. (1m) 
  7. Automatic generation of trees, mazes, complex spaces. (3m) 
  8. Algorithmic modification of existing shapes, such as bevels, geometric duals, and polyhedron stellation. (2m) 
  9. Shapes that morph: Rearranging vertices on the fly (5m) 
  10. Questions (5m) 

The ideas demonstrated in the talk are written against OpenGL 2.1, but written
in a 'mostly OpenGL 3' style, using vertex buffer objects or vertex arrays.

The demo code uses pyglet to create a window and handle GUI events, and uses
PyOpenGL for the majority of OpenGL calls, since it provides a more friendly
and Pythonic interface. In the performance-sensitive inner render loop,
however, I use pyglet's slightly more bare-bones OpenGL bindings.

However, the majority of the talk focuses on the manipulation of abstract data
structures to represent geometry, which is not affected by these or other
OpenGL library choices.

This is a substantially improved version of the talk 'Flying High: Hobbyist
OpenGL from Python', previously presented at EuroPython 2010.
