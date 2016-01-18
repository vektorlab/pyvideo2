---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=i6ah40KmwV8"'
ThumbnailUrl: 'http://i2.ytimg.com/vi/i6ah40KmwV8/hqdefault.jpg'
date: '2012-10-31'
speakers: [Christian Kauhaus]
tags: [icinga, ' monitoring', ' nagios', ' plugin']
---
Auch wenn in der letzten Zeit sehr viel Bewegung in die Monitoring-Szene
gekommen ist (#monitoringsucks etc.), werden die Platzhirsche Nagios/Icinga
und ihre Standards auf absehbare Zeit nicht verschwinden. Das Nagios-Plugin-
API stellt eine sehr weit verbreitete Schnittstelle zur Anbindung einzelner
Checks an Monitoring-Systeme dar. Obwohl das API in den Grundzügen sehr
einfach ist, ist der Programmieraufwand für vollständig konforme Plugins
erstaunlich hoch.

Die [_nagiosplugin_-Bibliothek](http://pypi.python.org/pypi/nagiosplugin/)
nimmt dem Entwickler viele Details ab, so dass er sich auf den Inhalt seiner
Checks konzentrieren kann. Der Vortrag führt in das Schreiben von Nagios-
kompatiblen Plugins ein, zeigt den typischen Aufbau von Nagios-Plugins und das
Grundprinzip eigener Plugins. Die Konfiguration und der Betrieb von
Monitoring-Systemen im Großen sollen nicht thematisiert werden.

Eine Einführung stellt die notwendigen Elemente wie Klassengerüst,
Messwerterhebung, Ranges, Statusausgabe und Performancedaten sukzessive in
aufeinander aufbauenden Beispielen vor, so dass am Ende ein einfacher, aber
praktisch einsetzbarer Check entsteht.

Der Teil über fortgeschrittene Aspekte und Stolperfallen reißt Einzelbeispiele
zu Themen wie mehrere Datenquellen, Timeouts, Auswertung wachsender Logfiles
und Checks mit "Gedächtnis" an und zeigt typischen Fehlerquellen auf.

Den Abschluss bildet ein kurzer Ausblick auf die weitere Entwicklung der
_nagiosplugin_-Bibliothek.

