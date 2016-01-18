---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=Vjslvo8atfw"'
ThumbnailUrl: 'http://i.ytimg.com/vi/Vjslvo8atfw/hqdefault.jpg'
date: '2014-07-24'
speakers: [Simon Cross]
tags: []
---
43% of the world's population live on less than €1.5 per day.

The United Nations defines poverty as a "lack of basic capacity to
participate effectively in society".  While we often think of the poor
as lacking primarily food and shelter, the UN definition highlights
their isolation. They have the least access to society's knowledge and
services and the most difficulty making themselves and their needs
heard in our democracies.

While smart phones and an exploding ability to collect and process
information are transforming our access to knowledge and the way we
organize and participate in our societies, those living in poverty
have largely been left out. This has to change.

Basic mobile phones present an opportunity to effect this change
[3]. Only three countries in the world have fewer than 65 mobile
phones per 100 people [4]. The majority of these phones are not
Android or iPhones, but they do nevertheless provide a means of
communication -- via voice calls, SMSes [6], USSD [7] and instant
messaging.

By comparison, 25 countries have less than 5% internet penetration
[5].

Vumi [1] is an open source text messaging system designed to reach out
to those in poverty on a massive scale via their mobile phones. It's
written in Python using Twisted.

Vumi is already used to:

  * provide Wikipedia access over USSD and SMS in Kenya [8].
  * register a million voters in Libya [10].
  * deliver health information to mothers in South Africa [9].
  * prevent election violence in Kenya [11].

This talk will cover:

  * a brief overview of mobile networking and cellphone use in Africa
  * why we built Vumi
  * the challenges of operating in unreliable environments
  * an overview of Vumi's features and architecture
  * how you can help!

Vumi features some cutting edge design choices:

  * horizontally scalable Twisted processes communicating using RabbitMQ.
  * declarative data models backed by Riak.
  * sharing common data models between Django and Twisted.
  * sandboxing hosted Javascript code from Python.

Overview of challenges Vumi addresses:

*Scalability*: Vumi needs to support both small scale applications (demos, pilot projects, applications tailored for a particular community) and large ones (things that everyone within a country might use). We address this using Twisted workers that exchange messages via RabbitMQ and store data in Riak. Having projects share RabbitMQ and Riak instances significantly reduces the overhead for small projects (e.g. its not cost effective to launch the recommended minimum of 5 Riak servers for a small project).

*Barriers to entry*: Often the people with good ideas don't have access to one of many things needed to run a production system themselves, e.g. capital, time, stable infrastructure. We address this by providing a hosted Vumi instance that runs sandboxed Javascript applications. All the application author needs is their idea, the ability to write Javascript and upload it to our servers. The target audience here is African entrepreneurs at incubator spaces like iHub (Nairobi), kLab (Kigali), BongoHive (Lusaka) and JoziHub (Johannesburg).

*Unreliable third-party systems*: It's one thing for parts of ones own system to go down, it's another for crucial third-party systems to go down. Vumi takes an SMTP-like approach to solving this and uses persistent queues so that messages can back up in the queue while third-party systems are down and be processed when they become available again. We also feedback information on whether third-party messaging systems have accepted or reject messages to the application that initiated them.

Vumi is developed by the Praekelt Foundation [2] (and individual contributors!).

  [1]: <http://vumi.org/> "Vumi"
  [2]: <http://praekeltfoundation.org/> "Praekelt Foundation"
  [3]: <http://www.youtube.com/watch?v=0bXjgx4J0C4#t=20> "Spotlight on Africa"
  [4]: <http://en.wikipedia.org/wiki/List_of_countries_by_number_of_mobile_phones_in_use>
  [5]: <http://en.wikipedia.org/wiki/List_of_countries_by_number_of_Internet_users>
  [6]: <http://en.wikipedia.org/wiki/Short_Message_Service>
  [7]: <http://en.wikipedia.org/wiki/Unstructured_Supplementary_Service_Data
  [8]: <http://blog.praekeltfoundation.org/post/65981723628/wikipedia-zero-over-text-with-praekelt-foundation>
  [9]: <http://blog.praekeltfoundation.org/post/65042080515/mama-launches-healthy-family-nutrition-programme>
  [10]: <http://www.libyaherald.com/2014/01/01/over-one-million-register-for-constitutional-elections-on-final-sms-registration-day/#axzz2sroHcg00>
  [11]: <http://blog.praekeltfoundation.org/post/51210616848/the-texting-will-never-be-done-peace-messages-in-kenya>