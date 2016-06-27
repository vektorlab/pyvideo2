---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: 'https://www.youtube.com/watch?v=u44L-l3RPy0'
Speakers: [Reinhard Wobst]
Tags: []
ThumbnailUrl: 'http://i2.ytimg.com/vi/u44L-l3RPy0/hqdefault.jpg'
Title: 'OpenOffice-Dokumente selbst modifizieren'
date: '2012-10-31'
---
Der Vortrag stellt eine Python-Klasse vor, die das fast beliebige Modifizieren
von Open/LibreOffice-Dokumenten bequem ermöglicht. Es geht mehr um die
Vorstellung einer Methode als um ein fertiges Werkzeug. So manche Aufgabe
lässt sich damit erheblich einfacher bewerkstelligen als mit Makros oder über
die pyUNO-Schnittstelle.

Hat man eine größere Zahl von ODF-Files (also im Open Document Format) oder
ein großes ODF-Dokument an vielen Stellen in gleicher Weise zu bearbeiten, ist
das ermüdend, zeitaufwändig und fehleranfällig. Wozu gibt es Computer?
Open/LibreOffice erlaubt zwar Makros, doch deren Leistung ist beschränkt, und
die pyUNO-Schnittstelle ist kompliziert, schlecht dokumentiert und noch nicht
ausgetestet.

Es geht auch anders: ODF-Files sind Zip-Archive von XML-Files, und diese
lassen sich mit Pythonskripten einfach bearbeiten. Das ODF-Format ist relativ
leicht zu verstehen (der Standard ist gut lesbar), der Phantasie des Anwenders
sind keine Grenzen gesetzt - sei es, um manuelle Formatierungen zu markieren,
in bestimmte Tabellen Spalten einzufügen oder diese um Zeilen zu ergänzen,
deren Berechnung partout nicht ins Konzept der Calc-Formeln passen will.

Dabei sind allerdings einige kleine Stolpersteine zu beachten, auf die der
Vortrag hinweist. Die hier vorgestellte Klasse ist eine mögliche Methode, um
sich auf die "wesentlichen Dinge" konzentrieren zu können.
