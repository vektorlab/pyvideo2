---
Category: 'EuroPython 2012'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=gmIG56Hf9dc"'
Speakers: [J Leidel, P Wassibauer]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/gmIG56Hf9dc/hqdefault.jpg'
Title: '"How to bootstrap a startup using django"'
date: '2012-07-04'
---
Based on our (Philipp Wassibauer and Jannis Leidel) experiences building
Gidsy.com this talk will give you valuable insight as to how your
infrastructure will evolve and how to set up the basic components
(Loadbalancer, Webservers, DB, Caching, Celery, CDN, …) of your site. Outline:
Basic project layout - How to handle different configurations and package your
project to make it easy to deploy and install. A basic timeline of how your
infrastructure needs will evolve - Starting from the initial 1 server setup we
will talk about how and when to scale out your servers. Replicate production
environments in development - We developed a way to have all your services
(Webserver, Celeryd, Solr, Cache, Compass compiler, …) running using one
management command. Setting up Chef recipes to provision your servers. Dealing
with cloud based servers - Tips and tricks on how to manage your cloud based
server using tools like Instagrams ec2-ssh. Automating deploying to a bigger
infrastructure (5+ servers) - Once the infrastructure becomes larger the
deployments become more tedious. There are a few automation tools for these
scenarios like the Etsy Deployinator. Tips on performance - How to find and
remove performance bottlenecks.

