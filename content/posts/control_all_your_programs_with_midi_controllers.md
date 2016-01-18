---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: '"http://youtu.be/p2CsRZoatc8"'
ThumbnailUrl: 'http://i.ytimg.com/vi/p2CsRZoatc8/hqdefault.jpg'
date: '2014-09-13'
speakers: [Tobi Wulff]
tags: [talk]
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Tobi Wulff:
Control All Your Programs with MIDI Controllers
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Saturday, 13 Sep 2014 - Track 1
http://kiwi.pycon.org/

**Audience level**

Intermediate

**Description**

MIDI devices are commonly used to provide input to audio applications, e.g. to play a synthesizer via a keyboard or to control a mixer in an audio workstation. This talk will show you tools for receiving input and processing messages, and how to control all of your programs with minimal configuration effort, the advantage being that not every single program has to be made natively MIDI aware.

**Abstract**

This talk will give a quick overview of the MIDI protocol and controllers which are commonly used to provide input to audio applications. These controllers can have the form of a musical keyboard, a mixer with knobs, sliders and buttons, or a combination of those. Some other variants use touch-sensitive trackpads or look like a drum kit. Then, the talk will go over the following tools: Python (duh), mididings (to receive and manipulate MIDI messages), xte (send keystrokes and mouse events to the Linux Xorg server) and some other necessary programs such as jackd to virtually connected MIDI inputs and outputs. I'll describe the steps needed to bring all those tools together and make it extensible to (hopefully, eventually) work on other OS as well.

mididings provides a Domain Specific Language (DSL) for MIDI processing which will be introduced as part of this talk. If you are doing anything with MIDI devices (and other external devices apart from keyboards) and feel like they pose some limitations on you (for example not supporting different customisable button assignments on the device), this will be of interest to you. xte will be used in a very basic way but if you haven't heard of it and want to send events to your X server, this is a great program. The possibilities are endless and we haven't even combined all the tools yet. This is about to change in the next step of the talk. A live demo/video will demonstrate how it all comes together into one beautiful piece of ingenuity and software engineering.

Finally, I'll discuss pros and cons of this solution versus other possible methods including native MIDI device support for various programs.

**Slides**

https://speakerdeck.com/nzpug/tobi-wulff-control-all-your-programs-with-midi-controllers