---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=KaPUo3G9JWk"'
ThumbnailUrl: 'http://i.ytimg.com/vi/KaPUo3G9JWk/hqdefault.jpg'
date: '2014-07-23'
speakers: [Philip Brechler]
tags: []
---
GoldenEye is our solution for mobile front end tests. Testing on mobile devices can be quite devastating: On iOS you can write front test in JavaScript in Instruments but it is quite impossible to connect Instruments to you CI solution of choice. On Android the situation isn't much better.
Other front end test frameworks can work with mobile devices (or simulators) but they lack the ability to see. Of course you can check if a color is set correctly, if a frame has the right x and y coordinates but in a world of different screen sizes writing these tests can be quite challenging as well.
In the end you will always need to look on your screen again and again trying to spot any issues. 

GoldenEye takes a different approach. It does not need to run on your development computer, you don't need a Mac for running tests on iOS devices and you can have real touches on your controls. This is archived by using openCV and it's python bindings, Pythons's unittest module and the Tapsterbot, an OpenSource delta robot made with 3D printing and an Arduino controller. To write a test you just take some screenshots on your device, cut out the icons you need to tap or inspect and write a very simple unit test using a high-level API that takes away the hard parts.

WARNING: This talk features a real robot. In case of machine world-domination: RUN!