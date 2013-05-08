---
layout: forensics
category: forensics
title: RegRipperRunner
---

# {{ page.title }} #

RegRipperRunner is to replace the functionality of my RegExtract tool e.g. run plugin, run hive, run folder but using Harlan Carvey's regripper, which means it has the same functionality and plugins as regripper without me having to maintain all of the plugins nor navigate via the command line for the numerous plugins that are implemented for it. By its nature it includes some of the plugin browser (pb.pl) and rr.pl functionality which overlapped with the functionality of RegExtract.

## Features ##

- Run single plugin
- Run multiple plugins
- Run against single hive
- Run against all hives in a folder
- Quickly modify the filter lists

## Third party ##

- [NLog](http://github.com/NLog/NLog) : Logging
- [ObjectListView](http://objectlistview.sourceforge.net/cs/index.html) : Data viewing via lists 
- [Registry](https://github.com/woanware/Registry): Binary registry hive parser (woanware)
- [Regripper](https://code.google.com/p/regripper/downloads/list): RegRipper (Harlan Carvey/keydet89)
- [Utility](http://www.woanware.co.uk): Misc functions (woanware)

## Requirements ##

Microsoft .NET Framework v4.5 

## Download ##

- [Source Code](https://github.com/woanware/RegRipperRunner)
- [Binaries (v0.0.2)](/downloads/autorunner.v.0.0.2.zip)
