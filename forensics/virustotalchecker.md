---
layout: forensics
category: forensics
title: virustotalchecker
---

# {{ page.title }} #

virustotalchecker is a .Net port of Didier Stevens [virustotal-search](http://blog.didierstevens.com/2012/05/21/searching-with-virustotal/) tool. I originally wanted the ability to provide a large list of hashes and get the results, along with caching to speed the process up as VT has a 4 requests per minute limit. I hadn't realised that Didier's tool did cache, by that time I had already written this.

The tool requires an API key from Virus Total. Once you have a valid key then add it to the Settings.xml e.g.

    <ApiKey></ApiKey>

## Features ##

- SQL CE database for caching of results
- CSV output

## Third Party Libraries ##
- [CommandLine](https://github.com/gsscoder/commandline): Used for command line parsing
- [JSON.Net](http://json.codeplex.com/): JSON library for importing a virustotal-search pickle file
- [MS SQL CE](http://www.microsoft.com/en-us/download/details.aspx?id=30709) : Access to MS SQL CE session database
- [NPoco](https://github.com/schotime/NPoco) : Easy access to SQL CE data
- [Utility](http://www.woanware.co.uk) (woanware) : My helper library
- [VirusTotal.NET](https://github.com/woanware/VirusTotal.NET) : Fork from https://github.com/Genbox/VirusTotal.NET, with new API's, caching etc

## Requirements ##

.Net 4.5

## Download ##

- [Source Code](https://github.com/woanware/virustotalchecker)
- [Binaries (v1.1.4)](/downloads/virustotalchecker.v1.1.4.zip)