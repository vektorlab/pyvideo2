---
Category: 'DjangoCon AU 2013'
Copyright: 'CC-BY-SA'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=RnMsobX3soE'
Speakers: [Greg Turner]
Tags: []
ThumbnailUrl: 'http://i1.ytimg.com/vi/RnMsobX3soE/hqdefault.jpg'
Title: 'Unleash the ponies! Using FeinCMS to add content tools that users love to
  any Django model'
date: '2013-07-05'
---
Site editors often struggle with editing rich content and managing variations in layout in Django admin. By rich content we mean text, images, video, tables, and so on. Trying to squeeze all this content into a single rich-text editor is like trying to jam a magical pony into a dog kennel. A better approach is to use a rich content framework like FeinCMS. FeinCMS is a sensible, flexible framework which allows rich content of any shape to be manipulated within any Django model in your project.

This talk describes what FeinCMS does and how it works, and most importantly whether it should be pronounced to rhyme with "Vein" or "Vine". The talk is supported with working example code that shows the progression of a FeinCMS project through several levels of functionality, plus some real-world demonstrations of fully-developed functionality.

A FeinCMS Document model is just like any Django model, except it has one or more 'templates'. Each 'template' has one or more regions, and each region is a place where an unlimited amount of rich content types can be added, removed or rearranged to form the content in that region. This is all wrapped up in a nifty lightweight Javascript interface for Django's admin, and a surprisingly simple implementation at the database level.

The types of content available in a given region is defined by a collection of abstract Django models (e.g. one model to represent a passage of text, another model to represent an image, and so on). Developers are free to define their own FeinCMS content types, using all the usual features of Django models.

At the HTML template level, each FeinCMS content item renders a standard template, and can optionally render different templates in different circumstances.

This flexibility allows Django developers to quickly design and build CMSes that match the content and layout perfectly, meaning happier content editors, fewer maintenance headaches and greater magical pony freedom.
