---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=zVPfVkC5qDk'
Speakers: [Valerio Maggio]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/zVPfVkC5qDk/hqdefault.jpg'
Title: 'Scikit-learn to "learn them all'
date: '2014-07-24'
---
**Machine Learning** is about *using the right features, to build the right 
models, to achieve the right tasks* [[Flach, 2012]][0]
However, to come up with a definition of what actually means **right** for 
the problem at the hand, it is required to analyse 
huge amounts of data, and to evaluate the performance of different algorithms 
on these data.

However, deriving a working machine learning solution for a given problem 
is far from being a *waterfall* process. 
It is an iterative process where continuous refinements are required for the 
data to be used (i.e., the *right features*), and the algorithms to apply 
(i.e., the *right models*).

In this scenario, Python has been found very useful for practitioners and 
researchers: its high-level nature, in combination with available tools and 
libraries, allows to rapidly implement working machine learning code 
without *reinventing the wheel*.

[**Scikit-learn**](http://scikit-learn.org/stable/) is an actively 
developing Python library, built on top of the solid `numpy` and `scipy` 
packages.

Scikit-learn (`sklearn`) is an *all-in-one* software solution, providing 
implementations for several machine learning methods, along with datasets and 
(performance) evaluation algorithms.

These "batteries" included in the library, in combination with a nice and intuitive
software API, have made scikit-learn to become one of the most popular Python 
package to write machine learning code.

In this talk, a general overview of scikit-learn will be presented, along with 
brief explanations of the techniques provided out-of-the-box by the library.

These explanations will be supported by working code examples, and insights on 
algorithms' implementations aimed at providing hints on 
how to extend the library code.

Moreover, advantages and limitations of the `sklearn` package will be discussed 
according to other existing machine learning Python libraries
(e.g., [`shogun`](http://shogun-toolbox.org "Shogun Toolbox"), 
[`pyML`](http://pyml.sourceforge.net "PyML"), 
[`mlpy`](http://mlpy.sourceforge.net "MLPy")).

In conclusion, (examples of) applications of scikit-learn to big data and 
computational intensive tasks will be also presented.

The general outline of the talk is reported as follows (the order of the topics may vary):

*   Intro to Machine Learning
    *   Machine Learning in Python
    *   Intro to Scikit-Learn
*   Overview of Scikit-Learn
    *   Comparison with other existing ML Python libraries
*   Supervised Learning with `sklearn`
    *   Text Classification with SVM and Kernel Methods
*   Unsupervised Learning with `sklearn`
    *   Partitional and Model-based Clustering (i.e., k-means and Mixture Models)
*   Scaling up Machine Learning
    *   Parallel and Large Scale ML with `sklearn`

The talk is intended for an intermediate level audience (i.e., Advanced).
It requires basic math skills and a good knowledge of the Python language.

Good knowledge of the `numpy` and `scipy` packages is also a plus.

[0]: http://goo.gl/BnhoHa "Machine Learning: The Art and Science of Algorithms that Make Sense of Data, *Peter Flach, 2012*"
