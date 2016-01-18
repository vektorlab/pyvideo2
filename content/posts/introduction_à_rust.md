---
Category: 'PyCon FR 2013'
Copyright: ''
Language: 'French'
SourceUrl: '"https://www.youtube.com/watch?v=qjxihcTJZ34"'
ThumbnailUrl: 'https://i.ytimg.com/vi/qjxihcTJZ34/maxresdefault.jpg'
date: '2013-11-30'
speakers: [Simon Sapin]
tags: []
---
Rust est un langage de programmation « systèmes » qui se veux sûr, concurrent, et pragmatique. Un de ses objectifs est de remplacer C/C++ dans les domaines où un langage plus « haut niveau » tel que Python n'est pas adapté : noyau de système d'exploitation, système temps-réel, moteur de navigateur web, etc.

Servo, un projet de Mozilla Research, est un moteur de rendu pour le web (tout comme Gecko est le moteur de Firefox) écrit en Rust et conçu pour tirer parti autant que possible du matériel moderne (multi-cœur) grâce aux fonctionnalités concurrentes de Rust.

- Présentation du langage: typage statique, sûreté et justesse vérifiés par le compilateur, pointeurs uniques, pointeurs empruntés, tranches de vecteurs, etc.
- État du projet (pré-1.0)
- Comment Servo gère les changements dans le langage et la bibliothèque standard.
- Mon ressenti après avoir travaillé sur Servo et WeasyPrint (Python), deux implémentations des même spécifications CSS.
- Une suite de tests basées sur des données, et partagée entre plusieurs implémentations.
- Comment utiliser Rust et Python dans le même programme, avec CFFI
- Courte introduction à la théorie des types, et aux types algébriques de données.
- Les types « sommes » sont des « unions taggées » en C, et des enum en Rust. (Plus général que Enum dans la PEP 435.) Pourrait-on avoir quelque chose de similaire en Python ?