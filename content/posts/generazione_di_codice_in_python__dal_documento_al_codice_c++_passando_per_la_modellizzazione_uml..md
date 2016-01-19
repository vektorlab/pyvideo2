---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'Italian'
SourceUrl: '"http://www.youtube.com/watch?v=jfBGt_g0Z4M"'
Speakers: [Francesco Bochicchio]
Tags: [api, ply]
ThumbnailUrl: 'http://i.ytimg.com/vi/jfBGt_g0Z4M/hqdefault.jpg'
Title: '"Generazione di codice in Python : dal documento al codice C++ passando per
  la modellizzazione UML."'
date: '2011-07-13'
---
Intendo presentare un programma di utilità che ho sviluppato per aiutare me e
i miei colleghi nel nostro attuale progetto.Space Software Italia Questo
programma esegue le seguenti attività: - Analizza un documento Microsoft Word
- generato automaticamente - allo scopo di estrarne le informazioni relative
alle strutture dati da usare per comunicare con dispositivi e/o programmi
software. Tali informazioni sono memorizzate in un modello UML, generato
interfacciandosi con il CASE tool usato in azienda (Rational Rose). - Utilizza
i dati in un modello UML - di solito una versione migliorata a mano di quello
generato automaticamente - per generare un set di classi C++, una per
messaggio, che forniscono i metodi per serializzare/deserializzare i messaggi
usando le API specifiche del progetto. Il programma è stato scritto in Python
2.x ed utilizza i seguenti moduli esterni: - pywin32: per interfacciare sia MS
Word che il tool CASE usando lo standard COM. - ply : per analizzare il file
in cui il tool CASE memorizza il modello,

