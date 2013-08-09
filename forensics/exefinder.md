---
layout: forensics
category: forensics
title: exefinder
---

# {{ page.title }} #

## Info ##

Sometimes it is hard looking for executables in strange places e.g. malware due to the number of paths extracted from an MFT or looking in a dir/file listing within a forensic tool. exefinder is a very simple tool that takes a list of file paths, identifies any .exe's, sorts them, and outputs a file, not rocket science and could be easily solved using the bash command line.

For example an MFT that contains 500K entries was reduced to about 2K.

## Third party ##

- [CommandLine](https://github.com/gsscoder/commandline): Used for command line parsing

## Requirements ##

Microsoft .NET Framework v4.5 

## Download ##

- [Source Code](https://github.com/woanware/exefinder)
- [Binaries (v1.0.1)](/downloads/exefinder.v.1.0.1.zip)
