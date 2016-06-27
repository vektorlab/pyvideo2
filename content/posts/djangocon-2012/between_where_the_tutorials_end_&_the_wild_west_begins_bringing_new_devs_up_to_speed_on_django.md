---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=OV5akJtAjgE'
Speakers: [Julia Grace]
Tags: [django]
ThumbnailUrl: 'http://i.ytimg.com/vi/OV5akJtAjgE/hqdefault.jpg'
Title: 'Between where the Tutorials end & the Wild West begins: bringing new devs
  up to speed on Django'
date: '2012-09-05'
---
This is a rough outline of how I learned Django; 4 months ago I was a total
outsider. Through this process I made mistakes, I had breakdowns, but I walked
away with a very solid understanding of Django and have proudly have written
thousands of lines of Python that are in production today. You'll leave this
talk with lessons on how to bring new developers to your team up speed on
Django.

  1. Read the Django docs (obviously, right?)
  2. Follow along building the sample application (Polls, Choices, yada yada).
  3. Decide to jump into writing production ready code. Have a breakdown. Feel like you're trying to boil the ocean with a lighter.
  4. Realize that building the sample app was cute but nothing compared to writing a real world application with real users and real constraints.
  5. Re-read the docs.
  6. Build a real Django app -- no more Polls. I decided to build a single-sign on application that allowed Etsy sellers to login and view all the photos of their all their listings in one place. I will give background as to why I chose this app, how I built it, and what it taught me.
  7. Start biting off small pieces of production code to figure out what the hell is going on. Learn about commonly used Django packages such as django-registration, django-profiles, taggit, etc. - and what happens when you need to modify the code of those packages.
  8. Attempt to boil the ocean, again. I needed to do a massive re- architecture of our application, combining several independent Django applications into a single, unified Django project. My first attempt totally failed. I will discuss why this was and key novice mistakes.
  9. Key realization that knowing Django != knowing Python
  10. "When you bang your head enough against the wall, eventually the wall comes down" -- me. I built a pretty kick ass Django application and I'm quite proud of.
  11. Celebrate (with lessons learned)!
