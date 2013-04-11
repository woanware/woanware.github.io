---
layout: forensics
category: forensics
title: PrefetchForensics
---

# {{ page.title }} #

## Info ## 

PrefetchForensics is an application to extract information from Windows Prefetch files. Prefetch files can obviously provide useful information in a forensic investigation like the date the application was last run and the number of times the application has run. The file format is relatively straight forward, although there are different binary formats between XP and Vista. 

PrefetchForensics will parse all prefetch files in a given directory, calculate the hash value using the determine algorithm, which should be the same value that is appended to the file name. The algorithm that generates the hash value is again different between XP and Vista e.g. 

- XP: (314159269×hash) mod 1000000007
- Vista: (37 * hash) + path[i];

Note that if there are multiple entries for the same file path, then the calculated hash value will probably be correct on one and not on any subsequent ones. It suggests that another parameter is being used when calculating the path hash. This parameter is currently unknown. If the application is a hosting application such as “rundll” or “mmc”, then the hash is formed with the exe hash + the hash of the case sensitive command line with a trailing space at the end: 

    HASH(\DEVICE\HARDDISKVOLUME1\WINDOWS\SYSTEM32\MMC.EXE) + HASH(C:\WINDOWS\system32\mmc.exe C:\WINDOWS\system32\drvmgmt.msc ) 

This information was identified through the CEIC 2008 presentation on Prefetch files. PrefetchForensics does not attempt to calculate this; therefore the calculated hash value is likely to be incorrect. The only way to validate the hash is to brute force the path and compare against the original hash to work out what application/binary was loaded by the host application. 

PrefetchForensics must be run as an administrator level user due to the low level operations performed by the application. Failure to run the application as an administrator level user may result in the application crashing. 

## Features ##

- CSV export
- HTML export
- Time zone offset support
- Parsed the date last run, number times run, path hash, calculates path hash as a secondary check, extracts the original path and the accessed files

## Screenshot ##

## Download ##
- [Binaries (v1.0.4)](/downloads/PrefetchForensics.v.1.0.4.zip)