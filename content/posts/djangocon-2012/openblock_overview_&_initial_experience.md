---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=nwr_G6Nln3s'
Speakers: [Colin Copeland, Karen Tracey]
Tags: [django, openblock]
ThumbnailUrl: 'http://i.ytimg.com/vi/nwr_G6Nln3s/hqdefault.jpg'
Title: 'OpenBlock: Overview & Initial Experience'
date: '2012-09-04'
---
# Abstract

What do you do if EveryBlock isn't available in your city? OpenBlock, released
to the community from the Knight-funded project, EveryBlock.com, is a
neighborhood news project aiming to provide a framework for "hyper-local"
civic data. Over the past few years, the open source project has been
maintained by the non-profit OpenPlans. Their goal was to simplify and
accelerate adoption of OpenBlock by making it easier to use. Today, Caktus is
working with Ryan Thornburg of the UNC School of Journalism and Mass
Communication to bring OpenBlock to rural North Carolina newspapers. Open
Rural aims to leverage OpenBlock to increase access to public records in small
communities. This talk focuses on our experience with OpenBlock as we work to
deploy OpenRural in North Carolina.

# Outline

## Introduction

  * What is OpenBlock?
  * How does it relate to/compare to EveryBock?
  * When/why might you want to incorporate OpenBlock into a site?
  * What have we (Caktus) be doing with OpenBlock?

## Geocoding

  * Geocoding is a hard problem to solve
  * String parsing
  * Places and locations
  * Street/block data
  * 3rd-party geocoder comparison

## Getting Started: Choosing Source for Street/Block Data

  * Pros and Cons of Census (Tiger) Data
  * Pros and Cons of Other Data Sources
  * Differences with county data and OpenBlocks preference for cities
  * Our Experience with Columbus County, NC

## Scrapers

  * What are they?
  * How do you write them?
  * Our Experience with Some Scrapers for Columbus County, NC
  * How we improve data accessibility with ScraperWiki

## The Missing Piece: Data Review and Analysis

  * OpenBlock handles scraping and public viewing, but is missing review and analysis
  * How successful was the geocoder?
  * How many news items were added this past week?
  * Why is my scraper failing to run?
  * Why did this address fail to geocode? How can I correct it?
  * Data Dashboard

## Adding OpenBlock to an Existing Site

  * Out-of-the-box views/templates
  * Our experience integrating with local online newspapers
  * Our OpenRural deployment setup

## Conclusion

  * State of the OpenBlock community
  * Our plans in North Carolina
