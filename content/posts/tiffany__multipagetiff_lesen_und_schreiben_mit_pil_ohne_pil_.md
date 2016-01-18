---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=qiZS1b_XFGs"'
ThumbnailUrl: 'http://i2.ytimg.com/vi/qiZS1b_XFGs/hqdefault.jpg'
date: '2012-11-01'
speakers: [Christian Tismer]
tags: [' distributed document capture', ' monkey-patching', multipage-tiff, ' pil']
---
Tiffany steht für beliebiges Tiff. Das kleine Modul löst eine grosse Menge

von Problemen, hat keine Abhängigkeiten, keine Binaries und läuft

überall wo Python läuft.

Bei der Entwicklung von Pydica (Distributed Document Capture) wurden wir

mit dem Problem konfrontiert, mehrseitige Tiff-Dateien anzuzeigen. Das

GUI-Toolkit PySide (Qt) unterstützt zwar Tiff, zeigt jedoch nur die erste
Seite.

Zudem behandeln wir Fax-komprimierte Dateien, was Qt aber unterstützt.

PIL verfügt über eine Bereinigung der Tiff-Tags, kommt aber nicht mit der

Fax-Kompression zurecht. Es gibt seit langem einen Patch dafür, jedoch ist

der Build-Prozess erschwert und zieht mit libtiff eine Kette von
Abhängigkeiten

nach sich.

Daher benutzt Tiffany einige wenige Dateien aus PIL ohne diese zu verändern
und täuscht

vor, die Tiff-Dateien zu entpacken, tut es aber nicht. Es werden lediglich die

Tiff-Tags ordentlich aufbereitet. Die komprimierten Daten werden so übernommen

wie sie sind. Beim Schreiben von Dateien werden daher lediglich die
vorhandenen

Daten in anderer Reihenfolge wieder zusammengesetzt.

Im Vortrag werde ich die Implementierung vorstellen sowie weitere
Alternativen,

die Zukunft von PIL sowie auf weitere Tips und Kniffe in unserem Projekt
eingehen.

