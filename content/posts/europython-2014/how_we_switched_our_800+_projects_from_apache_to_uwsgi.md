---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=e8Fz3bxPFC4'
Speakers: [Max Tepkeev]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/e8Fz3bxPFC4/hqdefault.jpg'
Title: 'How we switched our 800+ projects from Apache to uWSGI'
date: '2014-07-23'
---
The talk will start from describing the setup we had for the last 7 years, i.e. Apache with mod_wsgi for Python projects and mod_php4/5 for PHP projects + nginx. I will explain why we used this setup for so long time, what problems we faced with this setup and what solutions we tried to solve them before switching to uWSGI.

Then I will tell about uWSGI, what it is, how it works and what features it has. I will show the comparison of configuration files, how simple it is to configure uWSGI compared to Apache.

Lastly I will explain how we managed to switch all our 800+ projects developed over the years in 2 different languages with 2 major versions changed (PHP4/5 and Python2/3), how this switch simplified our development and administration of this projects, the improvements we got in memory management and other areas.

Of course I will concentrate mainly on our Python projects because it is EuroPython after all and not EuroPHP ;-)
