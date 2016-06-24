---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/424_backup-is-hard-let-s-go-shopping.mp4
Speakers: [Gary Bernhardt]
Tags: [backup, bigdata, bitbacker, pycon, pycon2011]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011BackupIsHardLetsGoShopping206.png'
Title: 'Backup Is Hard; Let''s Go Shopping'
date: '2011-03-11'
---
Backup Is Hard; Let's Go Shopping

Presented by Gary Bernhardt

We'll fly through the most clever bits of BitBacker, an online backup app
developed as a startup for three years and eventually abandoned. Highlights: a
hacked-up httplib/asyncore HTTP client; a real-life, HATEOAS-respecting
RESTful API, and an encryption scheme that can quickly diff a file system
against the server while leaking no information – not even file timestamps.

Abstract

This is the story of a solution to a huge problem: fast, secure online backup.
A single client generates a hundred gigabytes, millions of data chunks, and
thousands of file system snapshots. To appreciate the problem's scale,
consider that a Python array holding content hashes for 1,000,000 files
consumes 100 MB of memory. File hashes are only a portion of the required per-
file metadata, and that's only one for snapshot of thousands.

We'll tour the hard parts of this system with no apology for their difficulty.
The httplib/asyncore hybrid monster that served millions of parallel requests,
transparently retrying on failures and timeouts, with only 300 lines of
python. The RESTful API – fully respecting hypertext, with every request
safely repeatable, even POSTs, and not a single hard-coded URL in the client.
The encryption scheme that leaked nothing – not even modification times – but
could quickly diff local file systems against the server. And, that one time
that a client accidentally requested a 4.76 megabyte URL in production.

