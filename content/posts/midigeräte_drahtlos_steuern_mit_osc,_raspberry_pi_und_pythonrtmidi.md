---
Category: 'PyCon DE 2013'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=ZNsfvjeQ8cY"'
Speakers: [Christopher Arndt]
Tags: [diy, midi, musik, osc, raspberry pi, remote control]
ThumbnailUrl: 'http://i1.ytimg.com/vi/ZNsfvjeQ8cY/hqdefault.jpg'
Title: MIDI-Ger\xE4te drahtlos steuern mit OSC, Raspberry Pi und python-rtmidi\
date: '2013-10-16'
---
Mit der [python-rtmidi](https://pypi.python.org/pypi/python-rtmidi) Bibliothek lässt sich mit Python unter den drei gängigsten Betriebssystemen Windows, OS X und Linux auf MIDI-Schnittstellen zugreifen und MIDI-Daten senden und empfangen. Viele elektronische Musikinstrumente und anderes Soundequipment werden noch immer vorwiegend über das MIDI-Protokoll gesteuert und besitzen nur herkömmliche MIDI-Interfaces. Mit Hilfe einer auf *python-rtmidi* und [pyliblo](http://das.nasophon.de/pyliblo/) aufsetzenden Software, der *OSC-MIDI-Bridge*, einem Raspberry Pi und je einem billigen WLAN- und USB-MIDI-Interface, lassen sich solche Geräte kostengünstig in ein drahtloses Netzwerk einbinden und z.B. über Tablet-Computer steuern, auf denen entsprechende Software installiert ist, die OSC ([Open Sound Control](http://opensoundcontrol.org/)) unterstützt (z.B. [TouchOSC](http://hexler.net/software/touchosc) oder [TB MIDI Stuff](http://www.thiburce.com/TBStuff/)). Dies ist insbesondere für Situationen praktisch, in denen kein sperriger Desktop-Computer oder Laptop mit MIDI-Schnittstelle vor Ort vorhanden oder gewünscht ist.

Mit einer "Live"-Demonstration zeigt der Referent diese von ihm implementierte Software in Aktion (ca. 4 min) und erläutert dann kurz die dabei benutzten Protokolle (MIDI und OSC) (5 min), stellt die verwendeten Python-Bibliotheken *python-rtmidi* und *pyliblo* vor (4 min) und erläutert die eingesetzten Software-Techniken. Dabei wird insbesondere auf die asynchrone Behandlung von MIDI-Input und Output via des *multiprocessing*-Moduls der Standardbibliothek eingegangen (5 min). Abschliessend werden noch einige Anregungen für weitere Einsatzzwecke von *python-rtmidi* und der OSC-MIDI-Bridge gegeben (2 min).

*python-rtmidi* ist ein Python-Bindung für die C++-Bibliothek [RtMidi](http://www.music.mcgill.ca/~gary/rtmidi/index.html) und wurde mit [Cython](http://cython.org) realisiert. Die Software befindet sich noch im Alpha-Status, da momentan noch die Unterstützung der Kernel Streaming API unter Windows fehlt (Windows wird aber über das WinMM-Framework unterstützt). Die vorhandene Funktionalität ist jedoch stabil und es ist geplant, vor der PyCon.DE eine Beta-Version zu veröffentlichen. Die darauf aufsetzende OSC-MIDI Bridge ist bisher nur als Beispielskript in der *python-rtmidi*-Distribution verfügbar, wird aber stetig weiterentwickelt und voraussichtlich demnächst in ein eigenes Projekt ausgegliedert.