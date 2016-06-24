---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=IdVX4qHJXEY'
Speakers: [Adam Harvey]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/IdVX4qHJXEY/hqdefault.jpg'
Title: 'Four* non-cryptographic hash functions enter. One leaves.'
date: '2015-08-04'
---
When you say “hash function” in a room full of Python developers, people tend to think of the classics you get in hashlib: MD5, SHA-1, SHA-224, SHA-256, SHA-384, SHA-512, SHA-OHGODPLEASESTOP, and the like — cryptographic hash functions intended for cryptographic uses.

There’s another world out there, though: non-cryptographic hashes. Sometimes you just need to figure out if you’ve already seen a string or structure. Sometimes you need a basic checksum. Sometimes you need a hash that’s just fast and can fit into a 32 bit integer.

I’ll run through the state of the art in the world of non-cryptographic hashing — what your best options are, how they compare in terms of CPU and memory usage, and how they work. Who takes it? Whose mixing function reigns supreme?

Let’s find out.

* I’m saying “four”, but realistically I’m going to cover as many modern options as I can fit into the time available. Let’s say “four plus two or minus one” in reality.

