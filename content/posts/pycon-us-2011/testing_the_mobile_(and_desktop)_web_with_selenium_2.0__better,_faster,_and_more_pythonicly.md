---
Category: 'PyCon US 2011'
Copyright: 'Creative Commons Attribution-NonCommercial-ShareAlike 3.0'
Language: 'English'
SourceUrl: http://05d2db1380b6504cc981-8cbed8cf7e3a131cd8f1c3e383d10041.r93.cf2.rackcdn.com/pycon-us-2011/373_testing-the-mobile-and-desktop-web-with-selenium-2-0-better-faster-and-more-pythonicly.mp4
Speakers: [Jason Huggins]
Tags: [browsers, embedded, html5, pycon, pycon2011, selenium, webdriver]
ThumbnailUrl: 'http://a.images.blip.tv/Pycon-PyCon2011TestingTheMobileAndDesktopWebWithSelenium20524.png'
Title: 'Testing the Mobile (and Desktop) Web with Selenium 2.0 - Better, Faster,
  and more Pythonicly'
date: '2011-03-11'
---
Testing the Mobile (and Desktop) Web with Selenium 2.0 - Better, Faster, and
more Pythonicly

Presented by Jason Huggins

Selenium is a popular web application testing tool for acceptance testing
dynamic web applications. Selenium 2.0 has a different architecture that makes
it leaner, meaner, and more pythonic -- for testing desktop *and* mobile web
(iPhone/Android) apps. This talk will go into detail on how Selenium 2 works.
If you like testing and Python, you'll enjoy what's cooking in Selenium 2.

Abstract

Selenium was originally created by Jason Huggins and his team at ThoughtWorks
in 2004 as a tool for cross-browser acceptance testing of dynamic web apps --
apps that use JavaScript heavily on the client. Over the years, the Selenium
tool family has expanded to include a Firefox record and playback tool
(Selenium IDE), a Remote Control server that allows API access from any major
programming language, and a Grid server that allows tests to run in parallel
across many machines.

Despite it's widespread industry adoption, the Selenium project is far from
done. Selenium's goal is to drive any browser the same way an end user would
(e.g. opening pages, clicking buttons, entering text, etc.) with any
programming language on any OS platform. It's an ambitious goal, and with a
steady stream of new browsers (Chrome), new platforms (Android, iPhone), and
new HTML5 technologies (video, canvas, offline storage) to support, just
keeping up is an arduous task.

Astute observers will note, though, the bulk of Selenium's automation engine
is implemented in JavaScript, which is confined by the browser's security
sandbox in which it executes JavaScript code. That security sandbox ultimately
is at odds with Selenium's goal to drive the browser just as a user would. A
user has no problem interacting with security alerts for untrusted
certificates, or file upload dialog boxes, but Selenium can't deal with these
kinds of things easily without extra effort.

Enter WebDriver. There's a lot in common between the Selenium and WebDriver
projects. They're both tools for automated testing of web applications, and
both aspire to offer browser test automation from any language on any
platform. However, they do their thing in radically different ways. Selenium
uses the strategy that JavaScript is the one common tool available for
automating all browsers, even though its capabilities can be highly
constrained. Meanwhile, WebDriver leverages the strategy that acknowledges
different automation strategies work best for different browsers. COM works
best for IE on Windows, Apple Events for Safari on OS X. And Firefox, well,
the best way to natively automate Firefox is to turn it into a telnet server.
(But that's a whole other PyCon talk entirely!) WebDriver aims to natively
drive each browser the best way possible for maximum capability, then hiding
those differences between lower level C and C++ APIs, and finally exposing the
functionality through the appropriate C/C++ mechanism for each target
language, such as using ctypes for Python. With WebDriver's technical
approach, anything a user can do is now possible in test automation code.

This talk will go into detail explaining how Selenium and WebDriver (aka
Selenium 2) work, comparing the strengths and weaknesses of each tool's
approach to browser automation. The talk will then explain what Selenium 2.0
looks like and how to use it.

Talk outline:

  * Description of problem space 
    * More browsers 
    * More frequent browser releases 
    * HTML 5 - video, canvas, offline storage 
    * The web in more places - Mobile, Chrome OS 
  * Description of Selenium 
  * Strengths of Selenium 
  * Description of challenges for Selenium 1 
    * Javascript security sandbox 
    * Same origin policy / cross-site scripting 
    * OS-level popups 
    * Speed / stability 
    * Java as the cross-language integration point (aka Not Very Pythonic, eh?) 
  * Description of Selenium 2 (aka WebDriver) 
  * Strengths of Selenium 2 
  * How Selenium 2 is more pythonic 
    * (Lots and lots of example code goes here.) 
    * Spoiler Alert: No Java server required! 
  * How to test Android apps 
  * How to test iPhone apps 
  * Selenium development roadmap 

