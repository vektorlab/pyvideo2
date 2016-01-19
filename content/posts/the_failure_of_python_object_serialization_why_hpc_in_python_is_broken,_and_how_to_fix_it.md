---
Category: 'EuroScipy 2014'
Copyright: 'youtube'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=QvJmryCRfeY"'
Speakers: [Michael McKerns]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/QvJmryCRfeY/hqdefault.jpg'
Title: '"The failure of python object serialization: why HPC in python is broken,
  and how to fix it"'
date: '2014-10-22'
---
Parallel and asynchronous computing in python is crippled by pickle's poor
object serialization. However, a more robust serialization package would
drastically improve the situation. To leverage the cores found in modern
processors we need to communicate functions between different processes --
and that means callables must be serialized without pickle barfing.
Similarly, parallel and distributed computing with MPI, GPUs, sockets, and
across other process boundaries all need serialized functions (or other
callables). So why is pickling in python so broken? Python's ability to
leverage these awesome communication technologies is limited by python's own
inability to be a fully serializable language. In actuality, serialization
in python is quite limited, and for really no good reason.

Many raise security concerns for full object serialization, however it can
be argued that it is not pickle's responsibility to do proper
authentication. In fact, one could apply rather insecure serialization of
all objects the objects were all sent across RSA-encrypted ssh-tunnels, for
example.

Dill is a serialization package that strives to serialize all of python. We
have forked python's multiprocessing to use dill. Dill can also be leveraged
by mpi4py, ipython, and other parallel or distributed python packages. Dill
serves as the backbone for a distributed parallel computing framework that
is being used to design the next generation of large-scale heterogeneous
computing platforms, and has been leveraged in large-scale calculations of
risk and uncertainty. Dill has been used to enable state persistence and
recovery, global caching, and the coordination of distributed parallel
calculations across a network of the world's largest computers.

http://pythonhosted.org/dill

https://github.com/uqfoundation

http://matthewrocklin.com/blog/work/2013/12/05/Parallelism-and-Serialization/

http://stackoverflow.com/questions/19984152/what-can-multiprocessing-and-dill-do-together?rq=1

https://groups.google.com/forum/#!topic/mpi4py/1fd4FwdgpWY

http://nbviewer.ipython.org/gist/anonymous/5241793

