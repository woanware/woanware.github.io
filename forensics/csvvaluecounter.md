---
layout: forensics
category: forensics
title: csvvaluecounter
---

# {{ page.title }} #

## Info ##

Sometimes it is hard looking for values when there are large amounts of data e.g. hundreds of different mutex names, named pipes, file names etc. csvvaluecounter is a very simple tool that takes a CSV, gets the field value from the CSV as specified from the file, keeps count of each unique value, sorts by number, and then value, and outputs a file, not rocket science and could be easily solved using the bash command line.

## Third party ##

- [CommandLine](https://github.com/gsscoder/commandline): Used for command line parsing
- [LumenWorks.Framework.IO.Csv](http://www.codeproject.com/Articles/9258/A-Fast-CSV-Reader): Fast CSV reading

## Requirements ##

Microsoft .NET Framework v4.5 

## Download ##

- [Source Code](https://github.com/woanware/csvvaluecounter)
- [Binaries (v1.0.0)](/downloads/csvvaluecounter.v.1.0.0.zip)
