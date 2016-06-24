---
Category: 'PyCon Italia 2015'
Copyright: ''
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=pxBfDe7wiEo'
Speakers: [Daniel Pyrathon]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/pxBfDe7wiEo/maxresdefault.jpg'
Title: 'The Meta API: yesterday, today, and tomorrow'
date: '2015-05-29'
---
The Meta API is the core part of Django that enables introspection of the ORM with the rest of the system. The API allows different parts of the framework such as lookups, queries, forms, admin to understand and use the capabilities of every model.
As part of Summer of Code 2014 I refactored and redesigned some core parts of this API and, as the purpose of this talk, I plan on advocating how developers can benefit from this API in numerous ways: from understanding how Django’s model works, to enhancing your application through model introspection.
Moreover, I will give an overview of how we can create a custom store that can be plugged into Django, together with some code snippets and (maybe) a live demo.
This talk is an extension of the talk I did at Django Under the Hood, when the API was not finished yet. Now that the API has landed in master, I will also describe my process in getting involved into the Django community and how easy and rewarding it is to contribute to the project.
Objectives

Give a brief overview of what the Meta API is, it’s features and what can be done with it
Look at some of Django’s ORM code: from the model metaclass to the relation graph
Describe my experience in creating a custom Meta that talks to GMail through Django’s Model API (demo)
Define a small but concise guide on how to contribute to Django

