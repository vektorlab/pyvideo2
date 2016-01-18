---
Category: 'EuroScipy 2014'
Copyright: 'youtube'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=BiqPbiWv2hY"'
ThumbnailUrl: 'https://i.ytimg.com/vi/BiqPbiWv2hY/hqdefault.jpg'
date: '2014-10-22'
speakers: [Steve Braiser]
tags: []
---
This talk will discuss the design and implementation of a Python-based tool-set to aid in assessing the response of the UK's Advanced Gas Reactor nuclear power stations to earthquakes. The seismic analyses themselves are carried out with a commercial Finite Element solver, but understanding the raw data this produces requires customised post-processing and visualisation tools. Extending the existing tools had become increasingly difficult and a decision was made to develop a new, Python-based tool-set. This comprises of a post-processing framework ("aftershock") which includes an an embedded Python interpreter, and a plotting package ("afterplot") based on numpy and matplotlib.

The new tool-set had to be significantly more flexible and easier to maintain than the existing code-base, while allowing the majority of development to be carried out by engineers with little training in software development. The resulting architecture will be described with a focus on exploring how the design drivers were met and the successes and challenges arising from the choices made.