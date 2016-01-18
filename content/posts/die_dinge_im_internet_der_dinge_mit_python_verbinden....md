---
Category: 'PyCon DE 2013'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=TM7lO_B-BPw"'
ThumbnailUrl: 'http://i1.ytimg.com/vi/TM7lO_B-BPw/hqdefault.jpg'
date: '2013-10-17'
speakers: [Andreas Schreiber]
tags: [internet of things, mqtt, quantified self, raspberry pi, temperaturmessung]
---
Das Internet der Dinge besteht aus kleinen, manchmal intelligenten, Geräten und Sensoren, die über das Internet verbunden sind. Typische Sensoren sind Wettermessgeräte oder medizinische Geräte. Das Internet der Dinge wird nun bald real da sein, was durch günstige kleine Einplatinencomputer wie Raspberry Pi oder Arduino mit beeinflusst wird. Allerdings haben diese Geräte nicht viel Rechenleistung. Außerdem sind sie in machen Umgebungen auch nur mit eingeschränkter Netzwerkbandbreite angebunden. Um nun (viele) solche Geräte zu verbinden und Daten austauschen zu lassen sind sehr leichtgewichtige Protokolle und Implementierungen notwendig.

Der Vortrag ist über das Protokoll [Message Queuing Telemetry Transport](http://mqtt.org/) (MQTT), ein sehr geeignetes Protokoll zum Verbinden kleiner Geräte und Sensoren. MQTT basiert auf einer Publish/Subscribe-Architektur. Es eignet sich gut zum Schicken von Daten von Sensoren zu anderen Geräten. Zum Beispiel lassen sich Temperaturmesswerte von einem Temperaturfühler ohne viel Overhead zu einem Server schicken oder zu einem Smartphone als Push-Nachricht übermitteln. Ein andere Anwendung von MQTT sind Chat-Systeme, z.B. ist das [Facebook-Messaging](https://www.facebook.com/messages/) auf Basis von MQTT implementiert.

In dem Vortrag geht es vor allem um Open-Source-Implementierungen von MQTT. Speziell wird der freie MQTT-Broker [Mosquitto](http://mosquitto.org/) und dessen Python-Client-Bibliothek vorgestellt. Mosquitto ist eine leichtgewichtige Implementierung die effizient auf günstigen Einplatinenrechnern oder Smartphones läuft. An ein paar Bespielen in Python wird im Vortrag verdeutlicht wie leicht sich Anwendungen auf Basis von MQTT realisieren lassen: Die Übertragung von Temperaturmesswerten per Raspberry Pi zu einem Server, das Senden von Push-Nachrichten zu Android-Smartphones und das Senden von Smartphones aus einer Kivy-App heraus.