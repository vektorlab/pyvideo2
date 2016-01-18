---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=YkVscKsV_qk"'
ThumbnailUrl: 'https://i.ytimg.com/vi/YkVscKsV_qk/hqdefault.jpg'
date: '2015-08-04'
speakers: [Gregory Saunders]
tags: []
---
Scikit-learn's Random Forests are a great first choice for tackling a machine-learning problem. They are easy to use with only a handful of tuning parameters but nevertheless produce good results. Additionally, a separate cross-validation step can be avoided using the out-of-bag sample predictions generated during the construction of the forest, and finally they make it relatively easy to identify and extract the most important features of the sample data.

In this talk we’ll go through the process of using scikit-learn’s random forests using a financial data-set (of ASX equities) as an example. We’ll begin with a basic overview of the random forest algorithm and of the tuning parameters available and their impact on the effectiveness of the forest. Secondly we’ll go over the basic usage of scikit-learn’s random forests and in the process trouble-shoot some common problems such as dealing with missing sample data. Next we’ll discuss the use of out-of-bag sample predictions as a method for quickly performing cross-validation and optimising the tuning parameters. Finally we’ll look at how to extract information from the model that scikit-learn has generated, most notably the relative importances of the features in the sample data.