---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=ytgWM-WcJzs"'
ThumbnailUrl: 'http://i2.ytimg.com/vi/ytgWM-WcJzs/hqdefault.jpg'
date: '2012-10-31'
speakers: [Stefan Behnel]
tags: []
---
Keine PyCon(-DE) ohne Cython, die de-facto Standarderweiterungssprache für
Python. Diesmal geht es um ein paar neuere Spracherweiterungen zur Python-
Syntax, die den Cython-Compiler besonders attraktiv für High-Performance-
Computing machen: Parallele Schleifen mit OpenMP, effizientes Slicing mit
Memory-Views und generische Funktionen.

[Cython](http://cython.org "Web-Seite des Cython-Projekts") ist eine
Programmiersprache, die die Sprache Python um zusätzliche Features ergänzt.
Sie macht das Schreiben von schnellen Erweiterungsmodulen für CPython und das
Anbinden von externen nativen Bibliotheken (C/C++/Fortran/...) so einfach wie
Python selbst.

Dieser Vortrag gibt einen kurzen Einblick in Cython und speziell in die
Optimierung von schleifenbasierten Algorithmen über NumPy Arrays, mit denen
große Datenmengen effizient verarbeitet werden können. Dazu werden Memory-
Views verwendet, die mit Version 0.16 in Cython Einzug gehalten haben. Hinzu
gesellen sich parallele Schleifen, sowie generische Funktionen, die es dem
Compiler erlauben, einmal geschriebenen Code für verschiedene native
Datentypen zu optimieren.

Eine ausführliche Version dieses Vortrags mit entsprechenden Übungen wird
zusätzlich als Tutorial angeboten.

