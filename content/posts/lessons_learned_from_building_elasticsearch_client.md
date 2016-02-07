---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=rPpiOQNNm8U'
Speakers: ["Honza Kr\xE1l"]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/rPpiOQNNm8U/hqdefault.jpg'
Title: 'Lessons learned from building Elasticsearch client'
date: '2014-07-24'
---
Last year we decided to create official clients for the most popular languages, Python included.

Some of the goals were:

* support the complete API of elasticsearch including all parameters
* provide a 1-to-1 mapping to the rest API to avoid having opinions and provide a familiar interface to our users consistent across languages and evironments
* degrade gracefully when the es cluster is changing (nodes dropping out or being added)
* flexibility - allow users to customize and extend the clients easily to suit their, potentially unique, environment

In this talk I would like to take you through the process of designing said client, the challenges we faced and the solutions we picked. Amongst other things I will touch on the difference between languages (and their respective communities), the architecture of the client itself, mapping out the API and making sure it stays up to date and integrating with existing tools.
