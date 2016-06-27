---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=MVo0qEKK0wo'
Speakers: [Soren Hansen]
Tags: [openstack, packages, testing]
ThumbnailUrl: 'http://i.ytimg.com/vi/MVo0qEKK0wo/hqdefault.jpg'
Title: 'OpenStack Compute''s automated testing'
date: '2011-07-13'
---
When a patch is propoed against OpenStack compute (a.k.a. Nova) and it makes
it through our peer review process, our automated test system takes over:

  * It finds the approved patch on Launchpad;

  * An attempt to merge the patch is performed;

  * The unit tests are run;

  * A PEP-8 check is run;

  * The merge is completed, applying the patch to our trunk;

  * A tarball is built and published;

  * An Ubuntu source package is built for several editions of Ubuntu;

  * The source packages get uploaded to a PPA;

  * Once built, the packages are installed on a test setup;

  * A test battery is run against the installed "cloud".

I'll explain the various steps, showing how it works and attempt to
demonstrate it (Murphy's law permitting), and then I'll speak about the
benefits we've gotten from PPA's and working closely with Ubuntu.
