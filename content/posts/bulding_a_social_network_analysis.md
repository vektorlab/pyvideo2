---
Category: 'PyCon Italia 2015'
Copyright: ''
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=FQfFJ19g20I"'
ThumbnailUrl: 'https://i.ytimg.com/vi/FQfFJ19g20I/maxresdefault.jpg'
date: '2015-05-30'
speakers: [Luca Mearelli]
tags: []
---
Every conversation has a structure. The network formed by the persons who interact in the conversations inside an online community can thus be analysed with the tools of the network science to understand their characteristics. Enriching online conversations with social network analysis we hope to be able to give community moderators tools that could help them to build better communities and guide the collective intelligence processes inside them. The great vision in this is to be able to contribute to building the engines that could help us to build effective platforms for participatory democracy ( a better overview on these theme is explained by my colleague Alberto Cottica in this TEDx talk: https://www.youtube.com/watch?v=KKrM2c-ww_k  )

Edgesense is our attempt at making tools for social network analysis accessible to all those that could gain the most from them but maybe did not yet know their potential. Edgesense is built around a set of scripts that process the community data and extract the most relevant network metrics and the network structure and a dashboard that is able to present them giving a clear view of them. Through the dashboard community managers can for the first time see in a glimpse who is talking to who, which users are central to the community and those who are on the periphery. They can see which sub-communities are developing inside the larger online conversation and who is acting as a bridge between them.This is very useful to guide the conversation or to determine which users have the most authority (through measures of centrality or “pagerank")

Python has been central to the development of Edgesense it has made possible to create a processing pipeline that takes the  data from various sources (Drupal community sites, twitter conversations, mailing lists data) and builds the network of interactions among the users. Python has also enabled us to choose from a very rich library of social network analysis algorithms to calculate the metrics that we are presenting in the dashboard to help understand the social interactions.

During this talk we’ll look at which choices we were required when building a data processing application that takes real-life data, extracts useful informations and prepares t for visualisation. We’ll see a primer on the network science required to interpret the structure of the users community and how the algorithms and the metrics were chosen. We’ll also present the challenges that we are facing to extend Edgesense to ever larger communities.

The presentation will be useful to both developers interested in using python to do social network analysis and to those already skilled in it which could find inspiration in the problems we are trying to solve with Edgesense. 

Edgesense has been developed by Wikitalia within the CATALYST EC project on collective intelligence and it is available as open source software: https://github.com/Wikitalia/edgesense (an example of a live dashboard is available here: http://matera2019.edgesense.spazidigitali.com/ )
