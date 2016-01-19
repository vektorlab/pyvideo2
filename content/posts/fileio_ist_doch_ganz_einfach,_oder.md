---
Category: 'PyCon DE 2013'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=Qi8bXJ6b4vo"'
Speakers: [Christian Kauhaus]
Tags: [acid, "plattformunabh\xE4ngigkeit", systemprogrammierung, "zuverl\xE4ssigkeit"]
ThumbnailUrl: 'http://i1.ytimg.com/vi/Qi8bXJ6b4vo/hqdefault.jpg'
Title: '"File-I/O ist doch ganz einfach, oder?"'
date: '2013-10-16'
---
Der Vortrag soll Bewusstsein dafür schaffen, wann man sich aus einer komfortablen Umgebung (z.B. einem Application-Framework) in eine systemspezifische Domäne begibt. Aus meiner Erfahrung im DevOps-Umfeld sind mir viele Fälle bekannt, in denen Code auf Entwickler-Maschinen keine Probleme macht, sich aber auf produktiven Servern nicht ausreichend robust verhält. Die Eigenschaften von File-I/O in Python dienen dabei als durchgehendes Anwendungsbeispiel.

Der Vortrag gliedert sich in zwei Teile. Im ersten Teil möchte ich anhand von ausgewählten "Pannen" zeigen, wann ein *with open(...)* allein nicht ausreicht, da z.B. die Python-Standardfunktionen keine Zuverlässigkeit im Sinne der ACID-Eigenschaften gewährleisten. Im zweiten Teil geht um konkrete Programmiertechniken wie Write-Replace-Updates, Locking oder fsync, die die Robustheit von I/O ggf. unter Einschränkung der Plattformunabhängigkeit erhöhen. 

Der Anwendungsteil des Vortrags basiert auf Material aus meinem [Blogpost](http://blog.gocept.com/2013/07/15/reliable-file-updates-with-python/) zum gleich Thema.