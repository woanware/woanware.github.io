---
layout: network
category: network
title: SessionViewer
---

# {{ page.title }} #

SessionViewer is a PCAP TCP session reconstructor and viewer with the initial concept/code used from this [codeproject](http://www.codeproject.com/Articles/20501/TCP-Session-Reconstruction-Tool/) article. It has been rewrite numerous times to attempt to use a database as the storage, however, it has proven too slow, even with SQL Server, therefore multiple files are used that are generated with some pre-processing. 

To speed up the display of each session SessionViewer viewer produces a **large** amount of files, three files per session, a binary HEX version, an ascii version and a HTML viewer. The reason being that it reduces the processing when moving from session to session and adds only a minor overhead whilst performing the initial parsing. It also makes colourising of the conversations easier as it both sides of the network traffic.

## Features ##

- Fast
- HEX/Ascii/Colourised Views
- Quick view facilities e.g Q key to move up a session, A key to move down a session
- Excel like grid filtering (right click on the session list column headers)

## Third party libraries ##

- [ObjectListView](http://objectlistview.sourceforge.net/cs/index.html) : Data viewing via lists 
- [MS SQL CE](http://www.microsoft.com/en-us/download/details.aspx?id=30709) : Access to MS SQL CE session database
- [Be.HexEditor](http://sourceforge.net/projects/hexbox/) : HEX view of packet data
- [PCAPDotNet](http://pcapdotnet.codeplex.com/) : Parsing of PCAP files
- [NPoco](https://github.com/schotime/NPoco) : Easy access to SQL CE data
- [Winpcap](http://www.winpcap.org/) : Parsing of PCAP files
- [Utility](http://www.woanware.co.uk) (woanware) : My helper library
- [MaxMind GeoLite](http://www.maxmind.com): Geo IP locations

## Requirements ##

Microsoft .NET Framework v4.5

## Download ##

- [Source Code](https://github.com/woanware/SessionViewer)
- [Binaries (v1.1.0)](https://github.com/woanware/SessionViewer/releases/download/v1.1.0/SessionViewer.v1.1.0.zip)