---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=ZaCk9Gp8e-U"'
Speakers: ["Marc-Andr\xE9 Lemburg"]
Tags: [' interpreter', ' kompakt', ' laufzeitumgebung', ' open-source', ' python',
  virtualenv]
ThumbnailUrl: 'http://i3.ytimg.com/vi/ZaCk9Gp8e-U/hqdefault.jpg'
Title: '"eGenix PyRun - Python Laufzeitumgebung in einer Datei"'
date: '2012-10-31'
---
eGenix PyRun kondensiert eine komplette Python Laufzeitumgebung mit
Interpreter und Standardbibliothek in eine einzige sehr kompakte ausführbare
pyrun Programmdatei.

Da PyRun keine Installation benötigt und unabhängig von einer Python System
Installation arbeitet, bietet es sich damit als portable Lösung für Skripte,
Applikationen und in der Entwicklung als virtualenv Ersatz an.

PyRun ist nur 12-13MB groß, enthält aber den größten Teil einer üblicherweise
ca. 100MB großen Python Installation. Die Größe kann per gzexe oder upx auf
unter 4MB reduziert werden.

Es bietet damit eine ganze Reihe von Vorteilen gegenüber einer regulären
Python Installation. Hier die wichtigsten Aspekte:

* Sehr kompakt  
* Keine Installation oder Root Rechte notwendig  
* Kann unabhängig von einer System Python Installation verwendet werden  
* Bessere Startzeit als reguläres Python  
* Kompatibel mit distutils/setuptools/pip/etc.  
* virtualenv Ersatz

Derzeit unterstützte Systeme sind Linux, Mac OS X und FreeBSD. Es sollte aber
auch auf anderen Unix Systemen verwendbar sein. PyRun wird von eGenix unter
einer Open Source Lizenz verfügbar gemacht.

Der Vortrag wird das Projekt vorstellen, eine Anwendungsdemo zeigen und je
nach verfügbarer Zeit auch die Übersetzung demonstrieren.

