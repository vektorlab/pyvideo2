---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=9ZIPNWqjIEI"'
Speakers: [Ken Cochrane]
Tags: [django, pci-complicance]
ThumbnailUrl: 'http://i.ytimg.com/vi/9ZIPNWqjIEI/hqdefault.jpg'
Title: '"Building PCI compliant Django applications"'
date: '2012-09-06'
---
PCI DSS is a set of twelve different security standards that are required for
any organization that handles credit or debit card transactions. These
standards are created by the Payment Card Industry Security Standards Council
and they require all organizations to validate that they are compliant every
year.

Understanding these rules and how they effect you is sometimes a daunting
task. The goals of this talk will be the following:

  * Explain PCI DSS, and quickly go over the rules that will effect your application.
  * Show how to securely handle credit card transactions in your Django application.
  * Storing credit card information isn't ideal, but if you need to, I'll explain the different ways to securely store the data.
  * Go over the different ways to limit your PCI DSS liability (BrianTree, Akamai Edge Tokenization, Auth.net CIM)
  * Explore the different tools you will need in order validate your PCI compliance (Web application scans, IDS, Network Scan, firewalls)
  * How to be PCI Complaint in the cloud

I'll close out the talk with some of the details on how I haver personally
satisfied PCI DSS Requirements on my projects in the past. I'll cover some of
the tools and services that I used, and why I decided to use them.

At the conclusion of the talk you should have a better understanding of PCI
DSS, and what you need to do, in order for your Django application to be
certified as compliant.

