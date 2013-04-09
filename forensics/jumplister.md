---
layout: default
title: JumpLister
---

# JumpLister #

## Info ##

Jump Lists have been widely discussed within the forensic community, in particular on the win4n6 mailing list. Jump lists from a forensic perspective have been described as follows (Troy Larson): “put a MS-CFB (compound file binary file format) parser in front of the link file parser, you will have a tool that opens Windows 7 Jump lists” So that means they are a MS-CFB with N... MS-SHLLINK, so that’s what this application does. 

JumpLister is designed to open one or more Jump List files, parse the Compound File structure, then parse the link file streams that are contained within. It uses the LNK parser I wrote so stuff like object ID’s and MAC addresses are handled. The latest version also parses out the [DestList](http://www.forensicswiki.org/wiki/Jump_Lists) data and performs a lookup on the [AppId](http://www.forensicswiki.org/wiki/List_of_Jump_List_IDs). 

This functionality would not be possible without the hard work of the forensics community and the public release of the information on the [forensics wiki](http://www.forensicswiki.org/wiki/Jump_Lists). 

## Screenshot ##

## Download ##

- [v1.0.6](/downloads/JumpLister.v.1.0.6.zip)