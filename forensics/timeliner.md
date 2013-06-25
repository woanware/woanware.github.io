---
layout: forensics
category: forensics
title: Timeliner
---

# {{ page.title }} #

## Info ##

Timerliner is is designed to improve time line analysis for the output produced by the excellent log2timeline. There are plans to add support for log2timeline's replacement plaso in the near future once the release is stable.

The viewing and sorting of CSV files via spreadsheet software generally does not work well due to the volumes of data involved in modern time line analysis, which is where Timeliner comes in. The earlier releases of Timeliner used SQL Server LocalDB, which was fast but had a 10 GB database size limit, which became a problem when I tried to import a 15 million event time line! 

The implementation has it's limitations e.g. to support that amount of events and still perform fast queries I have had to remove support for jumping to page X etc, but it means it will page through the results taking under 1 second for 20000 results, under 3 for 100,000 results. The new query mechanism has meant I have had to remove the ability to apply custom sorts, a default sort on the time stamp is added by default. 

## Features ##

- Imports log2timeline, ntfswalk and fls
- Fast querying (under 1 second for 20000 results, under 3 seconds for 100,000 results)
- Supports huge data sets (tested with 15 million events)

## Third party ##



## Requirements ##

Microsoft .NET Framework v4.5 

## Installation/Running ##




