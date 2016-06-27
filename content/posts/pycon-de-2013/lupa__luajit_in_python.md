---
Category: 'PyCon DE 2013'
Copyright: ''
Language: 'German'
SourceUrl: 'https://www.youtube.com/watch?v=JreLvRxOF9M'
Speakers: [Stefan Behnel]
Tags: [lua, luajit, lupa]
ThumbnailUrl: 'http://i1.ytimg.com/vi/JreLvRxOF9M/hqdefault.jpg'
Title: 'Lupa - LuaJIT in Python'
date: '2013-10-17'
---
Der Python-Interpreter hat den Ruf, eine ausgereifte und grandios einfach zu verwendende dynamische Sprache und Laufzeitumgebung zu bieten, die für jede noch so [exotische Anforderung](https://xkcd.com/413/) eine Lösung bereit hält.

Ein oft genanntes Manko ist jedoch die begrenzte Performance des Interpreters für stark algorithmisch geprägte, kritische Teile von Anwendungen. Insbesondere hochdynamischer und generierter Code kommt hier schnell an seine Grenzen.

Auf der anderen Seite existiert mit LuaJIT2 eine sehr schnelle JIT-kompilierte Laufzeitumgebung der dynamischen Programmiersprache Lua, die bereits so manche Performance-Rekorde gebrochen hat und sich durch ihre geringe Größe leicht in andere Programme einbinden lässt. Das große Manko von Lua ist jedoch das Fehlen von Standard-Bibliotheken, die extrem begrenzten Sprach-Features und der daraus resultierende hohe Aufwand bei der Entwicklung größerer Anwendungen.

Mit [Lupa](https://github.com/scoder/lupa) steht eine Verbindung der beiden Programmiersprachen bereit, die es ermöglicht, aus Python heraus Lua-Code auszuführen und direkt mit diesem zu kommunizieren und Daten auszutauschen. So kann der größte Teil einer Anwendung in Python implementiert werden, und einzelne Aufgaben können von der schnellen LuaJIT-Umgebung übernommen werden.

Dieser Vortrag stellt das Projekt vor und gibt Einblicke in die Integration der beiden Programmiersprachen.
