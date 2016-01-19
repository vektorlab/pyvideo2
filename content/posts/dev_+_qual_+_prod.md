---
Category: 'PyCon DE 2012'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=hOqwe3wY7Yw"'
Speakers: ["Thomas G\xFCttler"]
Tags: [' deployment', ' linux', virtualenv]
ThumbnailUrl: 'http://i1.ytimg.com/vi/hOqwe3wY7Yw/hqdefault.jpg'
Title: '"dev --+ qual --+ prod"'
date: '2012-11-01'
---
Es wird das Konzept vorgestellt, wie man Projekte strukturieren kann um von
der ersten Minute an eine mind. dreistufige Landschaft (Entwicklung,
Qualitätssicherung, Produktiv) vorzusehen.

Die zentrale Rolle spielen getrennte Systemnutzer um isolierte Umgebungen zu
erstellen. Dieser Ansatz ist für Python-Server-Anwendungen wie z.B Django-
Anwendungen sehr gut anwendbar.

Seit einiger Zeit setzen wir getrennte Linux-Nutzer anstatt virtualenv ein.
Das zentrale Merkmal, ist der Name des Systemnutzers:

Namensschema des Linux-Nutzers: app_customer_stage

* app ist die Anwendung (zB cms)  
* customer ist ein Kürzel für den Kunden  
* stage ist d, q, p (dev, qual, prod).

Beispiel:

* mycms_customer1_d Entwicklungssystem  
* mycms_customer1_q Qualitätssicherung  
* mycms_customer1_p Produktivsystem

In einer zentralen Datei wird konfiguriert auf welchem Host welches System
läuft. Jedes System kennt das nächste System (Bsp dev->qual), so dass ein
Abgleich relativ einfach möglich ist.

Das simple System hat viele Vorteile, die ich in dem Vortrag vorstellen
möchte.

