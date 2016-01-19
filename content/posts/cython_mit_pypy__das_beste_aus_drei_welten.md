---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=IETT76NN6Z8"'
Speakers: [Stefan Behnel]
Tags: []
ThumbnailUrl: 'http://i2.ytimg.com/vi/IETT76NN6Z8/hqdefault.jpg'
Title: '"Cython mit PyPy - das Beste aus drei Welten"'
date: '2012-10-30'
---
Die Programmiersprache Cython ([http://cython.org](http://cython.org) "Web-
Seite des Cython-Projekts") ist das de-facto Standard-Tool um CPython um
nativen Code zu erweitern. Die Python-ähnliche Sprache macht schon seit
einigen Jahren das Schreiben von schnellen Erweiterungsmodulen für CPython und
das Anbinden von externen nativen Bibliotheken (C/C++/Fortran/...) so einfach
wie Python selbst und gleichzeitig so effizient wie C. Davon profitiert
besonders das weite Feld des High-Performance-Computing in Python
(NumPy/SciPy/Sage/...), aber auch zahllose andere Bereiche, die eine
effiziente Verarbeitung großer Datenmengen und die Anbindung von nativen
Bibliotheken an die Programmiersprache Python benötigen.

Die neueste Version des Cython-Compilers bietet erstmals auch Unterstützung
für PyPy an, eine alternative Python-Implementierung, die vor allem durch
ihren schnellen JIT-Compiler von sich reden macht. Dadurch kann einmal mit
Cython geschriebener und in C übersetzter Code sowohl in CPython als auch in
PyPy verwendet werden. So wird es beispielsweise möglich, in einer einzigen
Code-Basis effiziente Anbindungen externer Bibliotheken für beide
Laufzeitumgebungen zu entwickeln.

Dieser Vortrag von einem der Cython Core-Entwickler erklärt, welche
Fallstricke dabei noch auf Benutzerseite zu erwarten sind und gibt
Hilfestellungen beim Schreiben von Cython-Code, der sowohl in CPython als auch
in PyPy funktioniert.

