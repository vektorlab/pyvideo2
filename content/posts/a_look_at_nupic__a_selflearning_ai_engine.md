---
Category: 'Kiwi PyCon 2013'
Copyright: ''
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=rY7GLyxINFY"'
Speakers: [Tim McNamara]
Tags: []
ThumbnailUrl: 'http://i1.ytimg.com/vi/rY7GLyxINFY/hqdefault.jpg'
Title: '"A look at NuPIC - A self-learning AI engine"'
date: '2013-09-14'
---
@ Kiwi PyCon 2013 - Saturday, 07 Sep 2013 - Track 1

**Audience level**

Intermediate

**Abstract**

This talk will discuss the speaker's experience with NuPIC - http://numenta.org/nupic.html - for building useful artificial intelligence applications. In particular, the author will discuss developing damage and flood prediction models based on public sensor data.

About the tool

NuPIC is an open source implementation of algorithms which are inspired heavily by our understanding of how the neocortex organises information. NuPIC uses online (or continuous) learning, providing a prediction after every input is received. This is intended to mirror how human brains operate, by acting quickly on new information based on prior knowledge, while being able to adapt to it for the next bit of information. The other main features are the inclusion of a temporal dimension to learning, partitioning models into hierarchies of sub-models and representing knowledge within a sparse, distributed matrix modelled after the brain.

About the talk

The claims made in the documentation of NuPIC are very bold. The developers claim that models are able to be developed without needing to create training and testing sets. The models that are developed in this manner are supposedly self-learning. Surely, this must be exaggeration! This talk is a presentation of an evaluation of building models for two sets of input data, one relating to earthquakes and the other relating to flood levels.

The anticipated case studies

GeoNet provides an extensive archive of seismic data, along with associated damage reports from people affected by particular shakes. In principle, we could feed this historical data to NuPIC and then ask it to tell us how likely and how intense damage will be for any particular quake. Perhaps we could even use NuPIC to model predict the likelihood of multiple quakes within a cluster.

With information about rain levels available in near-real time from NIWA's climate database (Cliflo) and information about river catchments and historical from district councils, it is (in principle) possible to create a flood risk prediction model for one's own use.

**Slides**

https://speakerdeck.com/nzpug/tim-mcnamara-a-look-at-nupic-a-self-learning-ai-engine