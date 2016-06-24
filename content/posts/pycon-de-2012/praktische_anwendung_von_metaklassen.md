---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: 'https://www.youtube.com/watch?v=-dU-O8ksYDM'
Speakers: [Mirko Dziadzka]
Tags: [debugging, ' metaclasses']
ThumbnailUrl: 'http://i2.ytimg.com/vi/-dU-O8ksYDM/hqdefault.jpg'
Title: 'Praktische Anwendung von Metaklassen'
date: '2012-10-30'
---
Metaklassen (metaclasses) in Python werden oft als exotische Spracheigenschaft
betrachtet. Der Vortrag zeigt anhand konkreter Beispiele, wie sich Metaklassen
in realen Projekten zum Debuggen und zum Code vereinfachen einsetzen lassen.

# Praktische Anwendungen von Metaklassen

Python besitzt mit den Metaklassen ein sehr mächtiges Werkzeug, um orthogonale
Eigenschaften eines Programms zu Implementieren. Das Stichwort dazu lautet
"aspektorientiertes Programmieren". Leider werden Metaklassen aber oft als
komplex und schwierig angesehen.

Der Vortrag zeigt an einem konkreten Beispiel, wie sich durch die Verwendung
von Metaklassen Programmentwicklung vereinfachen kann. Konkret wird die
Implementation eines einfachen Debug- und Trace Frameworks vorgestellt.

Dieses erlaubt das nachträgliche instrumentieren von Klassen-Methoden, um eine
selektive Ablaufverfolgung von Methodenaufrufen auf Objekten ermöglicht. Dies
wird erreicht, ohne das diese Debug Aufrufe im normalen Quellcode erscheinen
oder bei nicht Benutzung Performance Auswirkungen haben.

