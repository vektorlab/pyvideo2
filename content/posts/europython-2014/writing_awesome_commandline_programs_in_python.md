---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=gR73nLbbgqY'
Speakers: [Mark Smith]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/gR73nLbbgqY/hqdefault.jpg'
Title: 'Writing Awesome Command-Line Programs in Python'
date: '2014-07-24'
---
Python is a great language for writing command-line tools - which is why so much of Linux is secretly written in Python these days. Unfortunately, what starts as a simple script can quickly get out of hand as more features are added and more people start using it!

The talk will consist of a tour through various useful libraries and practical code showing how each can be used, and include advice on how to best structure simple and complex command-line tools.

Things to consider when writing command-line apps:

* Single-file vs Multiple-file
* Standard library only vs. 3rd party requirements
* Installation - setup.py vs. native packaging

The different parts of a command-line program:

* Option Parsing:
    * Libraries: getopt, optparse, argparse, docopt
    * Sub-commands
* Configuration:
    * Formats: Ini file, JSON, YAML
    * Where should it be stored (cross-platform);
    * Having multiple configuration files, and allowing user config to override global config
* Output:
    * Colour - colorama
    * Formatting output for the user
    * Formatting output for other programs
    * How do you know when your output is being piped to another program?
    * Managing logging and verbosity
* Managing streamed input
* Exit values: What are the conventions?
* Interactive apps - REPL
* Structuring a bunch of programs/commands around a shared codebase.
* Command-line frameworks: clint, compago & cliff
* Testing command-line apps
* Writing command-line tools in Python 3 vs Python 2
