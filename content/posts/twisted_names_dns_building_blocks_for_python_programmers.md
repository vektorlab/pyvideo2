---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=kuSXK4gNYqw"'
Speakers: [Richard Wall]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/kuSXK4gNYqw/hqdefault.jpg'
Title: '"Twisted Names: DNS Building Blocks for Python Programmers"'
date: '2014-07-25'
---
# Description

My talk will consist of four main sections. Given the 30 minute time constraint,
I may shorten or drop the two introductory parts in favour of the narrative and
demonstration of interesting new APIs and code examples in the final two
parts. My experience of delivering a similar talk at PyconUK 2013 is that those
are the parts that will most interest the audience and prompt most audience
questions.

Here are my proposed sections with rough time allocations and descriptions:

## Introducing Twisted Names (0-5)

Twisted includes a comprehensive set of DNS components, collectively
known as Twisted Names.

-   <https://twistedmatrix.com/trac/wiki/TwistedNames>

I will begin the talk with a quick introduction to Twisted Names and its
capabilities, including one or two simple code examples.

## Introducing My Project (0-5)

With generous funding from The NLnet Foundation I am adding EDNS(0) and DNSSEC
client support in Twisted Names, including full DNSSEC verification and DANE
support.

In the talk I will quickly summarise the steps taken and lessons learned in
securing that funding, and hope to encourage the audience to seek funding to
support there own pet OSS projects.

## What's New in Twisted Names / Project Progress Report (10)

My project plan is divided into the following broad milestones.

1.  EDNS(0)

    1.  OPT record

    2.  Extended Message object with additional EDNS(0) items

    3.  EDNS Client

2.  RRSET handling

    1.  Canonical Form and Order of Resource Records

    2.  Receiving RRSETs

3.  DNSSEC

    1.  New DNSSEC Records and Lookup Methods

    2.  Security-aware Non-validating Client

    3.  Validating Client

4.  DANE

    1.  A twistd dns authoritative server capable of loading and serving TLSA
        records.

    2.  A Twisted web client Agent wrapper which performs TLSA lookup and
        verification of a server certificate.

    3.  A HostnameClientEndpoint which performs TLSA lookup and verification of a
        server certificate.

    4.  A command line tool for debugging TLSA records and for verifying a
        certificate file against a domain name.

    5.  A TLSA Record class for encoding and decoding TLSA bytes.

    6.  A TLSA lookup method which accepts port, protocol and hostname and constructs
        a suitable TLSA domain name.

In the talk I will quickly outline these goals, report on my progress so far,
and show running code examples to demonstrate the new APIs.

## Future Developments (5)

The aim of my project is to lay foundations that will eventually allow
end-to-end DNSSEC verification in all the core Twisted networking components,
including Twisted Conch (SSH), Mail (SMTP, POP3), Perspective Broker (RPC), Web
(HTTP, XML-RPC, SOAP), Words (XMPP, IRC).

Additionally I hope that this foundation work will encourage the development of
end-to-end DNSSEC verification in many of the Open Source and commercial
projects built on top of Twisted.

I will end the talk by outlining these exciting possibilities, and demonstrate
some code examples that illustrate these possibilities.

## Q & A (5-10)

I'm determined to leave at least five minutes at the end for audience
questions. At PyconUK 2013 I was frustrated because I ran out of time and ended
up answering questions outside the lecture theatre; questions which would have
been interesting to the whole audience.
