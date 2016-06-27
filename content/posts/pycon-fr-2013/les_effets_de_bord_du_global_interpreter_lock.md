---
Category: 'PyCon FR 2013'
Copyright: ''
Language: 'French'
SourceUrl: 'https://www.youtube.com/watch?v=eXY9CaFO254'
Speakers: [Adrien Guillo]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/eXY9CaFO254/maxresdefault.jpg'
Title: 'Les effets de bord du Global Interpreter Lock'
date: '2013-11-30'
---
"C'est seulement dans le cas de programmes multi-threadés qui passent beaucoup de temps au sein du GIL à interpréter du bytecode CPython que le GIL devient un goulot d'étranglement"

C'est ainsi que le GIL est présenté sur wiki.python.org jusqu'en 2009. Suite aux travaux de David Beazley (http://www.dabeaz.com) en 2009 et 2010, la communauté Python découvre que les effets du GIL vont au delà.

En effet, l'implémentation du GIL met en oeuvre une mécanique complexe qui ajoute un overhead important d'appels systèmes, particulièrement sur les processeurs multi-coeurs. De plus, le GIL pertube la livraison des signaux. Enfin, le GIL peut provoquer le scheduling de threads CPU bound avant celui de threads I/O bound, provoquant une dégradation des performances.

Ce talk s'appuyant sur les travaux de David Beazley (avec son aimable autorisation) tentera de donner une explication claire et détaillée aux effets de bord du GIL mentionnés ci-dessus.
