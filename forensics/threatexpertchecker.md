---
layout: forensics
category: forensics
title: threatexportchecker
---

# {{ page.title }} #

threatexpertchecker is a .Net application to check MD5 hashes against the ThreatExpert site. The application caches results for thirty days before rechecking an "known" hash.

## Features ##

- SQL CE database for caching of results
- CSV output

## Third Party Libraries ##
- [CommandLine](https://github.com/gsscoder/commandline): Used for command line parsing
- [MS SQL CE](http://www.microsoft.com/en-us/download/details.aspx?id=30709) : Access to MS SQL CE session database
- [NPoco](https://github.com/schotime/NPoco) : Easy access to SQL CE data
- [Utility](http://www.woanware.co.uk) (woanware) : My helper library

## Requirements ##

.Net 4.5

## Download ##

- [Source Code](https://github.com/woanware/threatexpertchecker)
- [Binaries (v1.0.2)](https://github.com/woanware/threatexpertchecker/releases/download/v1.0.2/threatexpertchecker.v1.0.2.zip)