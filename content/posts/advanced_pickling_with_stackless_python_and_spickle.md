---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=rwhZ4joMLsI"'
Speakers: [Anselm Kruis]
Tags: [packages, pickling, science, stackless]
ThumbnailUrl: 'http://i.ytimg.com/vi/rwhZ4joMLsI/hqdefault.jpg'
Title: '"Advanced Pickling with Stackless Python and sPickle"'
date: '2011-07-07'
---
Stackless Python supports pickling of a wider range of types than conventional
C-Python, including stack frames and code objects. On this basis it is
possible to extend further the pickle.Pickler class in order to serialise
classes, modules, packages up to certain limits. The [sPickle
package](http://pypi.python.org/pypi/sPickle) provides such an extended
Pickler. The code was developed as part of a commercial project and recently
released as free software by science + computing ag. Currently it requires
Stackless Python 2.7.

In my presentation, I'll first demonstrate some applications of the sPickle
package including serialisation of modules and executing parts of a program on
a remote computer using RPyC and Paramiko.

In the second part of my speech, I'll give some insight in the internal
operations of sPickle and the lessons learned during its development.
Extending the Pickler showed to be like opening a can of worms. You have take
care of many odds and ends to get it right. I'll point out some weak points in
the implementation of the conventional pickling code and I'll also show the
limits of the current sPickle implementation.

