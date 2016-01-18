---
Category: 'PyCon FR 2013'
Copyright: ''
Language: 'French'
SourceUrl: '"https://www.youtube.com/watch?v=QgDeh3IR0fs"'
ThumbnailUrl: 'https://i.ytimg.com/vi/QgDeh3IR0fs/maxresdefault.jpg'
date: '2013-11-30'
speakers: [Laurent Luce]
tags: []
---
En connaître plus sur l'implémentation d'un langage aide à être plus efficace quand on code. CPython est l'implémentation la plus utilisée et ses objets contiennent plein de merveilles. On découvrira quelques merveilles trouvées dans l'implémentation de la liste, du dictionnaire, de la chaîne de caractères et de l'entier.

On se posera les questions suivantes:

Qu'est-ce qui rend rapide la méthode "append" de la liste ?
Qu'est-ce qui est fait en interne pour accélérer la recherche d'une clé dans un dictionnaire ?
Qu'est-ce qui permet d'optimiser la mémoire utilisée par les entiers ?
On répondra à ces questions et on découvrira d'autres petites merveilles internes. Beaucoup de diagrammes seront utilisés pour être le plus clair possible. On montrera les différences entre Python 2.x et Python 3.x.

Sommaire:

Quelques merveilles internes de la liste:

- Le grand O de la méthode "append".
- L'algorithme de tri "timsort".

Quelques merveilles internes du dictionnaire:

- Redimensionnement du dictionnaire.
- Résolution des collisions.

Quelques merveilles internes de la chaîne de caractères:

- Partage des petites chaînes.
- L'algorithme de la méthode "find".

Quelques merveilles internes de l'entier:

- Partage des petits entiers.
- Groupes d'entiers.