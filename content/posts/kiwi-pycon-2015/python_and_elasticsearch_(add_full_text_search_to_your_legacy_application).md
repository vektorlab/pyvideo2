---
Category: 'Kiwi PyCon 2015'
Copyright: 'CC BY-SA'
Language: 'English'
SourceUrl: 'http://youtu.be/FM2e2J7OJpM'
Speakers: [Benoit Chabord]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/FM2e2J7OJpM/hqdefault.jpg'
Title: 'Python and Elasticsearch (Add Full Text Search to your legacy application)'
date: '2015-09-05'
---
At GrabOne we started to use Elasticsearch a year ago and integrate it with Django. The transition was pretty smooth.

## What Is Elasticsearch ?
* Open Source product https://www.elastic.co/products/elasticsearch
* Based on Apache Lucene index system
* Dristibuted, scalable and highly available
* Real time search and analytics capabilities
* RESTful API

## Integration With Python
* Because it is RESTful can be integrated with urllib
* Official Python connector maintained by the elasticsearch team https://github.com/elastic/elasticsearch-py
* Official Pythonic Query builder and Model mapper (ORM) https://github.com/elastic/elasticsearch-dsl-py

## GrabOne use case
* Started by redoing the search page
* Rebuilding the entire frontend using Elasticsearch as datasource for a Django website
