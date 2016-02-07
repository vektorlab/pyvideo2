---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=Eis-WqHda20'
Speakers: ["Domen Ko\u017Ear"]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/Eis-WqHda20/hqdefault.jpg'
Title: 'Rethinking packaging, development and deployment'
date: '2014-07-22'
---
Python is often mixed with other languages in development stack, nowadays it's hard to escape any JavaScript dependencies. If you add some C dependencies such as GStreamer to the stack, packaging becomes a burden.

While tweaking our packaging infrastructure will make things better, it's hard to fix fundamental problem of packaging with current ad-hoc solutions in Python domain.

Using Nix (http://nixos.org/nix/) for about a year gave me an insight that solving packaging problem at operating system level (bottom-up) is a better approach.

For example, wouldn't it be cool to have "virtualenv" implemented inside your package manager, so you could isolate also non-Python dependencies and not just Python packages for your project and not worry if system was updated?

We'll also show what benefits do we get by using the same tool for development and deployment and how little we have to do to deploy our application.

To see how Haskell community is touching the same subject, see blog post http://ocharles.org.uk/blog/posts/2014-02-04-how-i-develop-with-nixos.html

