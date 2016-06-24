---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=ZqKNDn56Aoo'
Speakers: [Lynn Root]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/ZqKNDn56Aoo/hqdefault.jpg'
Title: 'For lack of a better name(server): DNS Explained'
date: '2014-07-23'
---
Following instructions of what entries to create where is easy enough when using a PaaS.

But DNS is hard – deployment issues always seem to come down to DNS.

A solid understanding of DNS will not only help with deploying your applications, but will also give a greater understanding of how the internet works, and more generally, distributed systems.

In this talk, you will learn what DNS is, how it works and how to communicate with it, and how Python can make both interacting and spinning up your own DNS server simple (I swear!).  

Outline:

* Intro (1-2m)
* What DNS is (5 min)
    * URL -> IP addr, e.g. "phonebook" lookup (obligatory pun: Call me, Maybe?)
    * hierarchical system & resolution sequence (local DNS cache/resolver, ISP resolver, recursive DNS search)
    * popular types (primary, secondary/slave, forwarding, authoritative only, etc)
    * System components: what makes a DNS?
* How to communicate with DNS (3 min)
    * Protocol: UDP
    * Operations: CRUD
    * Resource records (A, AAAA, CNAME, SOA, SRV, etc)
    * tools: dig/nsupdate/nslookup
* Security overview (3min) (disclaimer: NOT a DNS security expert, not planning to get into the details here)
    * Server-Server, DynDNS: TSIG/GSS-TSIG
    * Server-Client: DNSSEC
* Python + DNS (10 min)
    * plain UDP query in Python (no 3rd-party libraries/no magic)
    * Interacting with a DNS w/ Python (dnspython.py)
    * Sample DNS server with Twisted
    * "fake" demo (either local or pre-recorded screen cast) of querying/updating/etc of the Twisted DNS
* Wrap up - resources page, github links, etc (1min)
* Q&A - ~5 min 