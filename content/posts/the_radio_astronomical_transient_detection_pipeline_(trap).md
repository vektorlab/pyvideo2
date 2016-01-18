---
Category: 'EuroScipy 2014'
Copyright: 'youtube'
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=_ExWz-j1ZhY"'
ThumbnailUrl: 'https://i.ytimg.com/vi/_ExWz-j1ZhY/hqdefault.jpg'
date: '2014-10-22'
speakers: [Gijs Molenaar]
tags: []
---
LOFAR, the Low Frequency Array, is an innovative new radio telescope in the Netherlands, which will continuously monitor the radio sky. The study of transient sources is one of the key science projects of LOFAR. Under this remit come all time-variable astronomical radio sources, including pulsars, gamma-ray bursts, X-ray binaries, radio supernovae, flare stars, and even exo-planets. With its continuous monitoring of a large area of sky, it is hoped that LOFAR will detect many new transient events, and provide alerts to the international community for follow-up observations at other wavelengths.

To detect and analyse transient sources we’ve created a software pipeline named TRAP. The TRAP is almost completely written in Python. In short the TRAP consists of:

* Source detection
* Storing to database
* Association in time and frequency (in database)
* Visualising results (webinterface)

Since the datarates in the pipeline are high, key in the design of our pipeline is that we move most calculations to the database. This implies complex and math heavy queries. To assist in managing these queries we use SQLAlchemy. TRAP can be used on various database backends like PostgreSQL, but also the less known MonetDB. MonetDB is a column store database which is believed to outperform traditional SQL databases on huge datasets. To interact with MonetDB we developed a Python API, SQLALchemy dialect and Django backend. For visualisation of the results we’ve created an interactive browser based web interface based on Django, bootstrap and highcharts. For parallising the image processing we use Celery. In my talk i’ll explain why we use these frameworks and dive in the internals of our pipeline.

Target audience is people that are interested in how to build a scientific processing pipline using off the shelf libraries.