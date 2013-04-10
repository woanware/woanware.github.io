---
layout: default
category: application
title: filefolderenum
---

# {{ page.title }} #

## Info ##

A number of tools exist that can perform file/folder enumeration but they generally suffer from false positives and cannot deal with custom 404 pages, this is where filefolderenum should create more consistent results. 

## Features ##

- Console
- SSL support
- Saves identified item to files
- Cookie support
- HTTP 1.0 and HTTP 1.1
- Basic Auth/NTLM Auth
- False postive and custom 404 detection

## Word Lists ##

It now uses a similar way to skipfish, which eliminates the need for multiple input files. The word list files now use the following format: 

    e:doc
    e:txt
    w:admin 
    w:test

Where the "e:" prefix denotes an extension and the "w:" prefix denotes a word. 

Have merged the skipfish "complete.wl" values with the existing lists, which increases the dirs/files from 243 to 2008 and the extensions from 82 to 130. These entries are in "Full.wl" There is a "Default.wl" which contains the old values contained in "Directories.txt", "Files.txt" and "Extensions.txt". 

There is "Sharepoint.wl" which contains the values from: fuzzdb\Discovery\PredictableRes\Sharepoint.fuzz.txt" 

If a word list file is loaded and no extensions are identified, then the directories list is cleared and all of the word list entries are deemed as files, this emulates the "-i" input file mode added in v1.0.7 

## Command Line Examples ##

    -h "www.test.co.uk" -c "files" --customonly 

The command line will perform the standard directory, file, extension checks for the "/files" directory and below 

    -h "www.test.co.uk" -c "files" -i "test.txt" 

The command line will perform checks using the "test.txt" input file for the "/files" directory and below. If the "test.txt" file consisted of the values "a,b,c", then the requests would be for: /a /b /c /files/a /files/b /files/c 

    -h "www.test.co.uk" -c "files" --customonly -i "test.txt" 

The command line will perform checks using the "test.txt" input file for the "/files" directory and below. If the "test.txt" file consisted of the values "a,b,c", then the requests would be for: /files/a /files/b /files/c 

## Download ##

[Binaries (v1.1.3)](/downloads/filefolderenum.v.1.1.3.zip)