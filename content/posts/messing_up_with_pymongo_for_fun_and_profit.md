---
Category: 'PyCon Italia 2015'
Copyright: ''
Language: 'Italian'
SourceUrl: '"https://www.youtube.com/watch?v=CQfPq6wXyJI"'
Speakers: [Alessandro Molina]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/CQfPq6wXyJI/maxresdefault.jpg'
Title: '"Messing up with PyMongo for fun and profit"'
date: '2015-05-30'
---
BSON (Binary JSON) è il formato di rappresentazione dei dati usato internamente da MongoDB per la trasmissione e rappresentazione dei documenti salvati nel database.
Ogni volta che si implementano delle API HTTP basate su MongoDB il driver (pymongo) riceve i dati in formato BSON e li deve convertire in un formato comprensibile da Python. Successivamente questi dati dovranno essere re-encodati nel formato usato dalle nostre API, solitamente JSON.
Per qualcosa come una API REST che solitamente è solo un proxy ai dati effettivi, l’encoding/decoding dance può arrivare a pesare pesantemente sulle performance riducendo il throughput del nostro API Server.
La presentazione mira a mostrare come studiando il funzionamento interno di PyMONGO ed alterandone alcuni flussi si può evitare in molti casi questo balletto e guadagnare sensibilmente in numero di richieste al secondo servite dal nostro ambiente.
