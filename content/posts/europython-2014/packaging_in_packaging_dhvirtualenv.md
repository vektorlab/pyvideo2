---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=d_jqe1O31X8'
Speakers: [Jyrki Pulliainen]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/d_jqe1O31X8/hqdefault.jpg'
Title: 'Packaging in packaging: dh-virtualenv'
date: '2014-07-24'
---
[Dh-virtualenv][1] is an open source tool developed at Spotify. We use it
to ease deploying our Python software to production. We built dh-virtualenv as a tool that fits our existing continuous integration flow with a dedicated sbuild server.
As we were already packaging software in Debian packages, the
aim of dh-virtualenv was to make transition to virtualenv based installations as smooth as possible.

This talk covers how you can use dh-virtualenv to help you deploy your
software to production, where you are already running a Debian-based system, such as Ubuntu, and what are the advantages and disadvantages of the approach over other existing and
popular techniques. We will discuss the deploying as a problem in
general, look into building a dh-vritualenv-backed package, and in the
end, look into how dh-virtualenv was actually made.

Goal is that after this presentation you know how to make your Debian/Ubuntu deployments easier!

[dh-virtualenv][1] if fully open sourced, production tested software,
licensed under GPLv2+ and available in Debian testing and unstable.

More information of it is also available in our [blogpost][2].


Talk outline:

1. Introduction & overview (3min)
    * Who am I?
    * Why am I fiddling with Python packaging?
    * What do you get out of this talk?
2.  Different shortcomings of Python deployments (5min)
    * Native system packages
    * Virtualenv based installations
    * Containers, virtual machine images
3. dh-virtualenv (10 min)
    * What is dh-virtualenv?
    * Thought behind dh-virtualenv
    * Advantages over others
    * Requirements for your deployment flow
    * Short intro to packaging Sentry with dh-virtualenv
4. How is it built? (10 min)
    * Debian package building flow primer
    * How dh-virtualenv fits that flow
    * What does it do build time and why?

[1]:http://github.com/spotify/dh-virtualenv
[2]:http://labs.spotify.com/2013/10/10/packaging-in-your-packaging-dh-virtualenv/
