---
Category: 'PyCon Italia 2015'
Copyright: ''
Language: 'Italian'
SourceUrl: 'https://www.youtube.com/watch?v=YGwciTWE60A'
Speakers: [Adriano Di Luzio]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/YGwciTWE60A/maxresdefault.jpg'
Title: 'Davvy - Django, WebDAV e (pessimo) stato dell''arte.'
date: '2015-05-29'
---
Davvy è un’applicazione Django che permette la gestione di servizi WebDAV.
Gli obiettivi del talk comprendono: fornire un’overview del protocollo WebDAV e mostrarne la nostra implementazione; mostrare la costruzione di un’applicazione Django che gestisca servizi basati su protocolli di questo tipo, in modo che sia estendibile a piacimento e pienamente configurabile (e quindi anche qualche buona regola da seguire nello sviluppo Django). 
Analizzare lo stato dell’arte e quindi, in particolare, come ogni client implementi, a proprio piacimento,  specifiche “personalizzate” del protocollo, risultando in una quasi impossibile interoperabilità e una scarsa compatibilità con i fornitori di servizi.
I prerequisiti necessari richiedono soltanto una conoscenza poco approfondita di Django.
Il talk includerà:

Dettagli sul protocollo WebDAV: cos’è, a cosa serve, come lo utilizziamo, e le alternative odierne.
Dettagli implementativi: come funziona WebDAV sotto il cofano, le estensioni che apporta ad HTTP, come utilizza l’XML e soprattutto, come utilizzare Django per gestirlo.
Django e WebDAV: la struttura nello specifico della nostra implementazione, il model, le view e l’implementazione di un’applicazione Django sui generis.
Scelte di implementazione, difficoltà tecniche e soluzioni: dove abbiamo utilizzato il database e dove invece abbiamo ritenuto più opportuno sfruttare le periferiche di archiviazione, i problemi che abbiamo incontrato durante lo sviluppo, e come li abbiamo risolti.
Il pessimo stato dell’arte: come ogni client implementi una propria versione “personalizzata” di WebDAV e come Davvy si adatta in mdo implicito ed automatico alle diverse richieste dei client. Esempi sui più noti client: Apple’s Calendar, Mozilla Thunderbird, e così via.
