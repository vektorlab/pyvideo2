---
Category: 'PyCon FR 2013'
Copyright: ''
Language: 'French'
SourceUrl: 'https://www.youtube.com/watch?v=iTU5CRuY96I'
Speakers: [David Cournapeau]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/iTU5CRuY96I/maxresdefault.jpg'
Title: 'Vagrant, packer et ruby pour automatiser des builds complexes'
date: '2013-11-30'
---
Vagrant, packer et un peu de ruby pour automatiser des builds complexes.

Introduction

Tout le monde n'a pas la chance de ne dépendre que de paquets 100 % python. Python est devenu un outil de choix pour le calcul numérique, mais des paquets tels que numpy, scipy ou scikit-learn dépendent de librairies C, C++ et même Fortran qui dépendent fortement des plateformes.

J'aimerais présenter les outils packer et vagrant comme une solution pour produire des builds 100 % reproductibles. S'appuyant sur la virtualisation, ils permettent d'appliquer les principes de reproduction non seulement pour unix, mais aussi os x et même windows.

Le concept de provisionnement, et son application au problème de "packaging"

Cette section présentera tout d'abord la nécessité de reproduction pour la compilation, et justifiera pourquoi les VM sont les outils les plus adéquats aujourd'hui si l'on veut supporter toutes les plateformes usuelles, en particulier windows:

- architectures "3-tier" pour le provisionnement
- outils disponibles pour chacune des 3 couches
- présentation de vagrant et packer

vagrant, un outil simple pour la réutilisation de VM

Cette section commencera par illustrer les problèmes usuels du partage des VM entre développeurs, et montrera comment vagrant peut résoudre ces problèmes:

- le provisionnement comme solution au manque de transparence usuel avec les VMs
- flexibilité et traçabilité grâce à la combinaison chef/puppet/salt + vagrant

packer, un complément à vagrant

Vagrant suppose l'existence de 'base box', qui sont des images d'OS avec juste ce qu'il faut pour "bootstrapper" la suite du provisionnement. Packer est un outil qui permet de créer ses propres images:

- illustration du fonctionnement de packer
- cibler plusieurs technologies de virtualisation à partir d' un même template: virtualbox, vmware, mais aussi ec2.

Example pour la compilation de paquets 'wheel' pour numpy/scipy

Cette partie sera plus didactique, et basé sur un exemple réel pour compiler un wheel de numpy et scipy sur windows. L'exemple utilisera à la fois vagrant, packer et chef.
