---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=Cgf73JmuINU'
Speakers: [F Haard]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/Cgf73JmuINU/hqdefault.jpg'
Title: 'Protocol specifications written in python'
date: '2012-07-04'
---
Rapidly updating the requirements and implementation of a machine-to-machine
communication protocol is hard in itself, and keeping a protocol specification
and documentation up-to-date is always a burden, and sometimes becomes an
impossibility. At Visual Units, when this became a problem with the protocol
between the embedded software and the fleet management server, we changed the
approach and specified the protocol in Python. This allows us to use the
specification directly when generating and parsing messages, as well as making
it possible to generate protocol documentation, and source code for our Java
(J2ME) client software. We implemented everything from scratch, and found it
surprisingly easy to do without documentation and specifications external to
The Code. This talk will focus on lessons learned and pitfalls found during
the implementation of this solution, with code examples from our current state
of art as well as showcases of some of the mistakes we made and the types of
magic used in different iterations - most notably metaclasses and the inspect
and imp modules. It will follow the evolution from the first (quite horrible)
attempts, to our current implementation. I will also discuss what has been
gained by adopting this solution and the tradeoffs that we have made. The
intended audience is developers and designers who work with and design
protocols, as well as developers with a general interest in code as
specification. This is not a presentation of a framework for use in any
application (although code is available), but an in-depth look at how far you
can go with custom-built tools.

