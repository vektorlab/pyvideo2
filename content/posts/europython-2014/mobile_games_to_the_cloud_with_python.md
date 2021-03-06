---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=wWypp2KexGs'
Speakers: ["Darko Roni\u0107", Mislav Stipetic]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/wWypp2KexGs/hqdefault.jpg'
Title: 'Mobile Games to the Cloud With Python'
date: '2014-07-22'
---
#### The Talk

This talk has two goals. Showing the audience the lessons we learned during a project which moved a simple mobile game to a server backend is our first intention. In addition to that we want to describe how such a system works in a real life example, to show which problems and which requirements arise in its creation. When the audience leaves the talk they will know how a real-life mobile game uses Python for powering the backend servers.

 
#### The Problem

Most of the game development for mobile devices is focused on running the game on the device. The game designers and game developers play a primary role in creating the product. The server backend plays a supporting role providing a multiplayer or social experience to the users. Indeed, at Nanobit Ltd., things were also done that way. We had a small Python infrastructure built around Django which provided a small portion of multiplayer experience for the players. The majority of development was still focused on playing the game on the device. That way of thinking was put to test when we decided to center our future games around the multiplayer experience. Due to the fact that our infrastructure at the time was not enough for what we had in mind, we had to start from scratch. The decision was made to use Python as the center of our new infrastructure.

In order to achieve it, a server backend was needed that would allow the game to be played “in the cloud” with the device only being a terminal to the player. Most of the game logic would have to be processed in the cloud which meant that each player required a constant connection to the backend and with over 100.000 players in our previous games that presented a challenge. How to build an infrastructure which can support that? Since every user action had to be sent to the backend how to process thousands of them quick enough? Those problems were big and were just the start.


#### The Solution

The design of the backend lasted for a couple of months and produced a scalable infrastructure based on “workers” developed in Python, “web servers” that use Tornado and a custom message queue which connected the two. The storage part is a combination of Riak and Redis. Since the backend is scalable new workers and new web servers had to be deployed easily so an orchestration module was build using Fabric. The scalability and launching of new workers and web servers was achieved using Docker for creation and deployment of containers. Each container presents one module of the system (worker, web server, queue). The end result can now support all of our future games and only requires the game logic of each game to be added to the workers.


#### The Technologies

* Python for coding the game logic, web servers. More than 90% of the system was written in Python.
* Fabric
* SQLAlchemy
* Riak
* Redis
* ZeroMQ
* nginx
* Docker
* Websockets
* AWS


#### The Lessons Learned

* How to tune the backend to handle the increasing number of active players.
* How to tackle the problem of frequent connection dropping and reachability issues of poor mobile device Internet connection in Tornado with a little help of Redis.
* How to prevent users from trying to outsmart the system by denying illegal moves.
* How to enable game profile syncing and live updating.
* Improving the performance of workers by prioritizing data being stored to databases (Riak, SQL).
* New issues and lessons show up all the time so there will definitely be more of them by the time of the conference.


#### Basic Outline

1. Intro (5 min)
    1. Who are we?
    2. How was Python used in our previous games
    3. Why we decided to change it all
2. Requirements (6 min)
    1. What was the goal of creating the game backend
    2. Why was Python our first choice
3. Python backend (14 min)
    1. The architecture of the backend
    2. Which technologies did we use and how were they connected together
    3. How the backend handles the game logic
    4. Lessons learned
4. Questions & Answers (5 min)
