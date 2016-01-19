---
Category: 'PyCon DE 2013'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=XOhRwhBnkf8"'
Speakers: [Dr. Jan Morlock]
Tags: [big data, disco, mapreduce, parallelisierung]
ThumbnailUrl: 'http://i1.ytimg.com/vi/XOhRwhBnkf8/hqdefault.jpg'
Title: '"MapReduce mit Disco"'
date: '2013-10-17'
---
Mit dem MapReduce-Verfahren können massive Datenmengen auf einem Rechencluster verarbeitet werden. Namensgeber und wichtige Bestandteile sind eine Map- und eine Reduce-Phase. Diese werden jeweils parallelisiert ausgeführt und ermöglichen somit eine optimale Auslastung der vorhandenen Ressourcen. Im Vergleich zu einer entsprechenden sequentiellen Implementierung können dadurch große Zeiteinsparungen erreicht werden. 

Mit dem freien Disco-Framework können MapReduce-Aufgaben leicht in Python erstellt werden. Beim Zugriff auf die Eingabedaten werden verschiedene Protokolle unterstützt. Während der Ausführung kann der Zustand des Rechenclusters sowie der Fortschritt der einzelnen Aufgaben mit Hilfe einer Weboberfläche überwacht werden. Ein verteiltes Dateisystem, das Disco Distributed Filesystem (DDFS), wird zur Speicherung der Zwischen- und Endergebnisse verwendet.