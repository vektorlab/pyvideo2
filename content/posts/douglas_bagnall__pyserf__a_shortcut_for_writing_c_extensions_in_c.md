---
Category: 'Kiwi PyCon 2009'
Copyright: 'No license (All rights reserved)'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/kiwi-pycon-2009/109_douglas-bagnall-pyserf-a-shortcut-for-writing-c-extensions-in-c.flv
Speakers: [Douglas Bagnall]
Tags: [extensions, kiwipycon, kiwipycon2009, pyserf]
ThumbnailUrl: 'http://a.images.blip.tv/Kiwipycon-DouglasBagnallPyserfAShortcutForWritingCExtensionsIn519-861.jpg'
Title: '"Douglas Bagnall - pyserf - a shortcut for writing C extensions in C"'
---
pyserf - a shortcut for writing C extensions in C

Presented by Douglas Bagnall

Abstract

There are many clever ways of connecting Python and C code together, and
pyserf is one of those. It is just a short script that parses a module outline
and produces an idiomatic template for a C extension providing the same
signatures, so all you need to do is write the bits that actually do stuff.

Outline

Pyserf is a tiny project that I wrote for my own use years ago and never
released because it is so obvious that dozens of better versions must exist.
The idea is simple -- you write an outline of a module like this:

    
    
    module documentation
    def top_level_function(int_a, float_b):
       "function documentation"
       return float_c
    
    class SomeModule:
       class documentation
       def foo(self, int_ants obj_zoo):
          method documentation
          return float_frogs
    

and pyserf uses the parsing modules in the standard library to generate a C
file that will compile to an extension providing the interface it describes,
with the documentation appearing in the right place and the type conversions
all properly handled. The generated file is not a hideous unreadable mess,
rather it is within a few characters of best practise according to the
official tutorial. Once you have this template, you abandon your outline and
write the middles of each function in C. In describing what pyserf does, this
talk will demonstrate what is required to write an extension in C by hand, and
show you some ways of using the standard libraries parsing modules.

[VIDEO HAS ISSUES: Sound and video are poor. Slides are hard to read.]

