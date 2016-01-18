---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=rilU44j_wUU"'
ThumbnailUrl: 'http://i.ytimg.com/vi/rilU44j_wUU/hqdefault.jpg'
date: '2014-07-23'
speakers: [Valentin Haenal]
tags: []
---
Compression is a technique to reduce the number of bits needed to
represent a given dataset. A very common use-case in the distributed
digital age is to reduce the size of files in order to reduce the time
and bandwidth requirements of sending a file from one location to
another.

There are a large variety of different algorithms and implementations of
so called "codecs" - a term is derived from the fact that programs that
implement a compression algorithm commonly constitute of both a
compressor and a corresponding decompressor. There are many different
special purpose compressors that exploit specifics in the structure of the
input data, for example: MP3, Ogg and FLAC for audio data such as music,
GIF, JPEG and PNG for images and  MPEG for encoding video. Also, there
are many general purpose codecs that make no assumptions about the
structure of the data, for example: Zlib(DEFLATE), Bzip2(BWT) and LZMA.

However, and due to the ever growing divide between memory access latency and CPU clock
speed a new use-case beyond faster file transfers and more efficient use
of disk-space has emerged: "in-memory compression".


Keeping data in RAM that is compressed also means that the CPU has to
do more work in order to make use of it.  However, if the compressor
is fast enough, this decompression overhead could pay off, and
applications could work with compressed data transparently, and so not
even noticing the slowdown due to the extra effort for
compression/decompression.

This technique can be very beneficial in a variety of scenarios where
RAM availability is critical.  For example, in-memory caching systems
like Memcached or Redis could store more data using the same resources
thereby optimizing resource usage.  Another use case is to use
compression for in-memory data containers, à la NumPy's ndarray or
Pandas' DataFrame, allowing for improved memory usage and potentially
allow for accelerated computations.

In our talk, we will explain first why we are in a moment of computer
history that [in-memory compression can be beneficial for modern
applications] [1].

Then, we will introduce [Blosc] [2], a high speed
meta-compressor, allowing other existing compressors (BloscLZ, LZ4,
Snappy or even Zlib) to leverage the SIMD and multithreading framework
that it provides and help achieving extremely fast operation
(frequently faster than a plain memcpy() system call).

Finally, we will show some existing data handling libraries ([Bloscpack] [3], [PyTables] [4], [BLZ] [5]) -- all written in Python -- that
already use Blosc today for fulfilling the promise of faster operations by
doing in-memory compressing.

[1]: http://www.pytables.org/docs/CISE-12-2-ScientificPro.pdf
[2]: http://www.blosc.org
[3]: https://github.com/Blosc/bloscpack
[4]: http://www.pytables.org
[5]: http://continuum.io/blog/blz-format