---
Category: 'PyCon FR 2013'
Copyright: ''
Language: 'French'
SourceUrl: '"https://www.youtube.com/watch?v=oQ17KDBr24I"'
ThumbnailUrl: 'https://i.ytimg.com/vi/oQ17KDBr24I/maxresdefault.jpg'
date: '2013-11-30'
speakers: [Victor Stinner]
tags: []
---
Les fuites mémoire en Python ne peuvent pas être analysées avec les outils traditionnels car Python repose sur les compteurs de référence. Je vais présenter des outils spécifiques à Python pour vous aider à localiser vos fuites mémoires.

- Consommation globale du processus (mémoire RSS)
- Comprendre les cycles de référence
- Générer une image représentant les liens entre les objets
- Utilisation de gc.get_objects() et calcul manuel de la taille des objets
- Tracer les allocations mémoires à leur création
- PEP 445: Add new APIs to customize Python memory allocators implementée dans Python 3.4
- Projet pytracemalloc