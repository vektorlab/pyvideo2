---
Category: 'DjangoCon 2010'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: 'http://blip.tv/file/4106752'
Speakers: [Jeff Balogh]
Tags: [casestudy, djangocon, djangocon2010]
ThumbnailUrl: 'http://a.images.blip.tv/Robertlofthouse-SwitchingAddonsmozillaorgFromCakePHPToDjango334.png'
Title: 'Switching addons.mozilla.org from CakePHP to Django'
---
Switching addons.mozilla.org from CakePHP to Django

Presented by Jeff Balogh

In January of 2010 Mozilla started switching addons.mozilla.org (AMO) from
CakePHP to Django. We see about 120 million web requests per month and 1.4
million visitors per day. This talk will be a case study of scaling and
deploying a large website (and getting faster than PHP) with MySQL, memcached,
virtualenv, Celery, Hudson, Redis, MongoDB, and more.

Abstract

To scale the backend of AMO, we rely heavily on caching in memcached (and soon
Redis) to keep the load off our database, and multidb to spread the load we
can't dump off on cache. Our caching ranges from object and query caching, to
template fragment caching, up to full response caching. Frontend caching is
external to Django and won't be covered. In addition, we work hard to measure
and improve raw speed. Hitting indexes and keeping datasets small is critical,
and the Django ecosystem has many great tools to help us profile.

We create development environments using pip and virtualenv, so we naturally
started using that setup to deploy the site in production. We ran into issues
creating a reliable environment with this method; switching to a separate
vendor repository solved our problems with only a small amount of added
effort. We update and deploy new code at least once a week, and have to deal
with the additional complication of managing and interacting with parts of the
PHP site that have not been ported over.

Apart from scaling and deployment, we've customized our application in ways
that could be interesting to other Django users:

  * Jinja is our templating engine (but we keep the admin working) 
  * Babel helps us localize the site in over 30 languages 
  * Sphinx (not the documentation tool) serves our search results 
  * Celery and RabbitMQ help us do offline processing 
  * Nose and Hudson help us get over 90% code coverage in tests 

