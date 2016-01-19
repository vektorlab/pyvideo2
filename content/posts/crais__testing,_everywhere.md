---
Category: 'PyCon Italia 2015'
Copyright: ''
Language: 'English'
SourceUrl: '"https://www.youtube.com/watch?v=8SIW_R6FP9E"'
Speakers: [Aniello Barletta]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/8SIW_R6FP9E/maxresdefault.jpg'
Title: '"CRAIS - Testing, everywhere"'
date: '2015-06-09'
---
CRAIS acts as an Appium (1) broker, in order to spawn Appium servers as selenium grid nodes with specific capabilities using:

* USB hotplug Mechanism for locally-connected devices, where CRAIS dinamically generate the node, registering itself to the hub,
* RPC invocation, where CRAIS spawns ad-hoc appium server instances. The RPC method could be used to use remote android devices connected to the server using a reverse-ssh tunnel.

CRAIS is based on:

* ZODB object database for device storage (for both Hotplug & RPC), ConfigObj for configuration management, Pyro4, a library that enables to build applications in which objects can talk to each other over the network,
* Cement as CLI framework.

CRAIS is implemented in order to use the same Object Database in both RPC & Hotplug mode.

(1) Appium is an open source test automation framework for use with native, hybrid and mobile web apps, used in B! to integrate Android / iOS testing in a QA automation infrastructure.

Prerequisites:

1. Selenium GRID specifications
2. Acceptance testing knowledge
3. Python multithreading & subprocess32 modules usage
