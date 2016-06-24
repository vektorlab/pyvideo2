---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=uBV_KKGzNqQ'
Speakers: [Tarashish Mishra]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/uBV_KKGzNqQ/hqdefault.jpg'
Title: 'Building Realtime Web Applications with WebRTC and Python'
date: '2014-07-25'
---
Introduction
===========
This talk will first introduce the audience to WebRTC and then discuss about how to implement the server side logic of a WebRTC app using Python. 

WebRTC is a free, open project that enables web browsers with plugin-less Real-Time Communications (RTC) capabilities via simple JavaScript APIs. What makes WebRTC special is that the data travels from one client to another without going through the server. 

The main functions of WebRTC can be broadly categorized into three types. 

- Access and acquire video and audio streams
- Establish a connection between peers and stream audio/video.
- Communicate arbitrary data.

WebRTC uses three different JavaScript APIs to perform these three functions. These APIs are:

- MediaStream (aka getUserMedia)
- RTCPeerConnection
- RTCDataChannel

MediaStream API performs the task of accessing the webcam and/or microphone of the device and acquire the video and/or audio stream from them. RTCPeerConnection API establishes connection between peers and streams audio and video data. This API also does all the encoding and decoding of audio/video data. The third API, RTCDataChannel helps to communicate arbitrary data from one client to the other.

There will be short demos to demonstrate the functionalities of these APIs.

Signaling and Session Control
========================

WebRTC uses RTCPeerConnection to communicate streaming data between browsers, but some sort of mechanism is needed to coordinate this communication and to send control messages. This process is known as signaling.

Signaling is used to exchange three types of information.

- Session control messages: to initialize or close communication and report errors.
- Network configuration: to the outside world, what's my computer's IP address and port?
- Media capabilities: what codecs and resolutions can be handled by my browser and the browser it wants to communicate with?

This can be implemented using any appropriate two way communication channel.

Implementing signaling in Python
==========================

Next, we will have a look at how to implement this signaling mechanism in Python. ( Demonstration with annotated code and live application.)

### Google AppEngine and the Channel API ###
Google AppEngine has a channel API which offers persistent connections between your application and Google servers, allowing your application to send messages to JavaScript clients in real time without the use of polling. We'll use this Channel API to build the signaling system of our WebRTC app on top of webapp2 and flask framework. 

### Flask and gevent ###
We'll implement the same signaling system again, this time on top of Flask using gevent for the persistent connection between the browser and our application. 

Outline of the talk
===============
### Intro (5 min) ###
- Who are we?
- What is WebRTC?
- Functions of WebRTC.

### WebRTC APIs and Demos (3 min) ###
- MediaStream (getUserMedia) API
- RTCPeerConnection API
- RTCDataChannel API

### Signaling in WebRTC Applications (3 min) ###
- What is signaling?
- Why is it needed?
- How to implement it?

### Implementation of signaling (16 min) ###
- Implementation using Google AppEngine and Channel API
- Implementation using Flask and gevent

### Questions (3 min) ###
