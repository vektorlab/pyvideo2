---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=0flbR0HNWBA'
Speakers: [Dougal Matthews]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/0flbR0HNWBA/hqdefault.jpg'
Title: 'Using asyncio (aka Tulip) for home automation'
date: '2014-07-25'
---
This talk will cover the new asyncio library in Python 3.4 (also known as Tulip) and will use the area of home automation as a case study to explore its features. This talk will be based on code using Python 3.3+.

Home automation is a growing area and the number of devices and potential applications is huge. From monitoring electricity usage to the temperature inside or outside your house to remote control of lights and other appliances the options are almost endless. However, managing and monitoring these devices is typically a problem that works best with event driven applications.

This is where asnycio comes in, it was originally proposed in PEP 3156 by our BDFL, Guido van Rossum. Asyncio aims to bring a clear approach to the python ecosystem and borrows from a number of existing solutions to come up with something clean and modern for the Python stdlib.

This talk will introduce asyncio and use it within the context of home automation and dealing with multiple event driven devices. Therefore we will cover asyncio and the lessions learned from using different devices in this context.

Some of the devices that will be used include:

 - Raspberry Pi
 - RFXCom's RFXtrx, USB serial tranciever.
 - Owl CM160 electricity tracker.
 - Oregon scientific thermometers.
 - Foscam IP cameras.

This talk will also briefly cover the previous solution I used which was developed with Twisted and compare it briefly with my new code using asyncio.
