---
Category: 'PyCon DE 2013'
Copyright: ''
Language: 'German'
SourceUrl: '"https://www.youtube.com/watch?v=2w7K5wUL9IE"'
ThumbnailUrl: 'http://i1.ytimg.com/vi/2w7K5wUL9IE/hqdefault.jpg'
date: '2013-10-17'
speakers: [Felix Huber]
tags: []
---
Field Programmable Gate Arrays (FPGA) werden normalerweise auf Registerebene programmiert mit Hardwarebeschreibungssprachen wie Verilog oder VHDL. Dies ist vergleichbar mit Assemblerprogrammierung eines Mikroprozessors. Die Sprache Handel-C (sic!) hat sich zum Ziel gemacht, Hardwarebeschreibung mit C-Syntax zu ermöglichen, unabhängig von der zu Grunde liegenden Hardware. Dazu muß das Problem die Synchronizität durch die inhärente Parallelität einer Hardwarefunktion gelöst werden. Mit Handel-C ist es nun möglich, einen Algorithmus in C zu schreiben, auf einem Rechner zu simulieren und anschließend aus dem identischen Quellcode eine Hardwareimplementierung zu synthetisieren. Dabei gehen die Vorteile einer Hochsprache nicht verloren, im Gegenteil: durch den global optimierenden Compiler werden weniger Ressourcen auf dem FPGA benötigt. Zusammen mit Bibliotheken für Fest- und Fließkommaarithmetik, Graphikausgabe und Tastatur bedient sich ein FPGA dann wie ein embedded Prozessor mit einem Geschwindigkeitszuwachs von Faktor 100.