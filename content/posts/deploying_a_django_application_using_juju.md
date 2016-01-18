---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: '"http://youtu.be/6hc8VkFeHjA"'
ThumbnailUrl: 'http://i.ytimg.com/vi/6hc8VkFeHjA/hqdefault.jpg'
date: '2014-09-14'
speakers: [Tim Penhey]
tags: [deploying, deployment, django, juju]
---
Juju is a service orchestration tool for deploying services into public or private clouds. The services that Juju deploys are described in Charms. A Charm should use the "best practice" for deploying the service. In the case of Django, this would be using gunicorn and nginx. I explain how the postgresql charm communicates with the django charm, and how I had to change my application's settings and urls to work with the django charm. The application that is deployed is a "proprietary" app, and as such, the deployment of the application itself is done with another charm. The interaction between the subordinate charms and the principal django charm are explained, and how the data is exchanged between the charms. As well as the deployment story, I also explain how application updates are deployed very simply.