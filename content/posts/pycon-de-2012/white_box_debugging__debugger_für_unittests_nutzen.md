---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: 'https://www.youtube.com/watch?v=26tmYQk2vI8'
Speakers: [Reinhard Wobst]
Tags: []
ThumbnailUrl: 'http://i3.ytimg.com/vi/26tmYQk2vI8/hqdefault.jpg'
Title: \"White Box Debugging\" - Debugger f\xFCr Unittests nutzen\
date: '2012-10-31'
---
"White Box Testing" ist das Testen von internen Zuständen zur Laufzeit,
während ubliche Unittests in der Regel nur Funktionen rufen. Man kann aber
mittels eines Debuggers White Box Testing durchführen - ein Pythonskript
erlaubt dies fur Python mit pdb wie auch für C/C++ - Programme mit gdb.

Unittests sind ohne Frage unerlässlich, aber oft aufwändig zu programmieren
und beschränkt aussagefähig, da in der Regel nur einzelne Funktionen oder
Module als Black Box getestet werden können. Nicht selten ist sogar
gesonderter Code notwendig, um sinnvolle Tests zu ermöglichen.

Aussagekräftiger und naheliegender wären Tests auf Werte mitten im Code, doch
solch eine Funktionalität bietet bisher nur die assert-Anweisung, die bei
Fehlern mit einem wenig aussagekräftigen Abbruch endet.

Die Idee des Python-Skripts "wbd" ("white box debugging") ist, aus Kommentaren
im Quelltext Konfigurationsfiles für Debugger zu erzeugen, so dass an
bedingten Breakpoints Tests stattfinden. Beim Fehler landet man gleich im
Debugger und kann die Umgebung analysieren.

Das funktioniert derzeit für Pythonskripte und C/C++-Programme und ist auch
gut als Hilfsmittel beim Debuggen selbst einzusetzen.

