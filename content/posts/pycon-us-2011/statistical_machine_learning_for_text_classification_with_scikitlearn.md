---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/417_statistical-machine-learning-for-text-classification-with-scikit-learn.mp4
Speakers: [Olivier Grisel]
Tags: [googlepredictionapi, machinelearning, nltk, pycon, pycon2011, scikit-learn]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011StatisticalMachineLearningForTextClassification447.png'
Title: 'Statistical machine learning for text classification with scikit-learn'
date: '2011-03-11'
---
Statistical machine learning for text classification with scikit-learn

Presented by Olivier Grisel

The goal of this talk is to give a state-of-the-art overview of machine
learning algorithms applied to text classification tasks ranging from language
and topic detection in tweets and web pages to sentiment analysis in consumer
products reviews.

Abstract

Unstructured or semi-structured text data is ubiquitous thanks to the read-
write nature of the web. However human authors are often lazy and don't fill-
in structured metadata forms in web applications. It is however possible to
automate some structured knowledge extraction with simple and scalable
statistical learning tools implemented in python. For instance:

  * guessing the language and topic of tweets and web pages 
  * analyze the sentiment (positive or negative) in consumer products reviews in blogs or customer emails 

This talk will introduce the main operational steps of supervised learning:

  * extracting the relevant features from text documents 
  * selecting the right machine learning algorithm to train a model for the task at hand 
  * using the trained model on previously unseen documents 
  * evaluating the predictive accuracy of the trained model 

We will also demonstrate the results obtained for above tasks using the
[scikit-learn](http://scikit-learn.sourceforge.net/) package and compare it to
other implementations such as [nltk](http://nltk.org/) and the [Google
Prediction API](http://code.google.com/apis/predict/).
