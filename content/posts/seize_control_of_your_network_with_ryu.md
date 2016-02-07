---
Category: 'Kiwi PyCon 2014'
Copyright: 'CC'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=JKBQ-2uiwcw'
Speakers: [Ewen McNeill]
Tags: [talk]
ThumbnailUrl: 'http://i.ytimg.com/vi/JKBQ-2uiwcw/hqdefault.jpg'
Title: 'Seize control of your network with Ryu'
date: '2014-09-13'
---
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
Ewen McNeill:
Seize control of your network with Ryu
= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = 
@ Kiwi PyCon 2014 - Saturday, 13 Sep 2014 - Track 2 
http://kiwi.pycon.org/

**Audience level**

Intermediate

**Description**

Ryu is an OpenFlow Network Controller written in Python, which provides a framework to build your own Software Defined Network (SDN) that can run at full wire speed, using modern network switches. Come learn how to leverage Python to instruct your network to filter, switch, and route traffic precisely the way you desire.

**Abstract**

OpenFlow [1] is an industry standard protocol for controlling modern network hardware (and software switches -- such as Open vSwitch [2] in Linux), down to installing specific forwarding or filtering rules ("flows") into the hardware forwarding plane. Together with a well written OpenFlow Network Controller it allows you to create an intelligent Software Defined Network (SDN).

Ryu [3] is a OpenFlow Network Controller framework, written in Python, that is already extremely capable and still being rapidly developed (new releases every month). It has been adopted by the OpenStack [4] project amongst many others. Ryu implements the OpenFlow wire protocols and allows you to write event driven "apps" as Python modules, each running in their own eventlet. It comes with lots of examples. Your own apps can dictate switch forwarding and filtering policy in advance, or respond to new types of packets as they arrive. This gives you fine grained programmatic control over your network.

The talk will provide a brief outline of a how a Software Defined Network using Openflow works, and an introduction to writing your own Ryu "app" in Python. Plus plenty of pointers so you can get started experimenting yourself. Become the mad genius taking total control of your network!

[1] https://www.opennetworking.org/
[2] http://openvswitch.org/
[3] http://osrg.github.io/ryu/
[4] http://www.openstack.org/

**Slides**

https://speakerdeck.com/nzpug/ewen-mcneill-seize-control-of-your-network-with-ryu