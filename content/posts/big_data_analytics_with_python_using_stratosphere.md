---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=J3RMB4HgcRw"'
ThumbnailUrl: 'http://i.ytimg.com/vi/J3RMB4HgcRw/hqdefault.jpg'
date: '2014-07-25'
speakers: [Chesnay Schepler]
tags: []
---
[Stratosphere](http://stratosphere.eu/) is implemented in Java. In 2013 we introduced support for writing Stratosphere programs in Scala. Since Scala also runs in the Java JVM the language integration was easy for Scala.

In late 2013, we started to develop a generic language binding framework for Stratosphere to support non-JVM languages such as Python, JavaScript, Ruby but also compiled languages such as C++. The language binding framework uses [Google’s Protocol Buffers](https://code.google.com/p/protobuf/) for efficient data serialization and transportation between the languages.

Since many “Data Scientists” and machine learning experts are using Python on a daily basis, we decided to use Python as the reference implementation for Stratosphere’s language binding feature.
Our talk at the EuroPython 2014 will present how Python developers can leverage the Stratosphere Platform to solve their big data problems.

We introduce the most important concepts of Stratosphere such as the operators, connectors to data sources, data flows, the compiler, iterative algorithms and more.
Stratosphere is a mature, next generation big-data analytics platform developed by a vibrant [open-source community](https://github.com/stratosphere/stratosphere). The system is available under the Apache 2.0 license. 

The project started in 2009 as a joint research project of multiple universities in the Berlin area (Technische Universität, Humboldt Universität and Hasso-Plattner Institut). Nowadays it is an award winning system that has gained worldwide attention in both research and industry.

A note to the program committee: As mentioned, the development of the Python language binding of Stratosphere has started a few months ago, therefore, the code is not yet in the main development branch. However, we are already able to execute the “Hello World” of big data, the “Word Count” example using the Python interface. See this example in the development branch: https://github.com/filiphaase/stratosphere/blob/langbinding/stratosphere-addons/stratosphere-language-binding/src/main/python/eu/stratosphere/language/binding/wordcountexample/WordCountPlan.py


Please contact us if you have any questions!