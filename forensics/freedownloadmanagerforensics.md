---
layout: forensics
category: forensics
title: FreeDownloadManagerForensics
---

# {{ page.title }} #

## Info ##

FreeDownloadManager is a free download manager and was mentioned on the [SANS forensics blog](https://blogs.sans.org/computer-forensics/2009/12/17/free-download-manager-log-extraction). The application stores its logs under "userprofile\Application Data\Free Download Manager". There are various different files stored, the main one of interest is "downloads.his.sav".

The file structure is like so: 

- 22 Bytes: "FDM Downloads History" + NULL
- 2 Bytes: Unknown (Was 93 or 0x5D)
- 2 Bytes: File Version (Currently 1)
- 4 Bytes: Num Records
Then follows the records. The record structure is so: 
- 4 Bytes: Length
- File Name
- 4 Bytes: Length
- Saved To Location
- 4 Bytes: Length
- URL
- 4 Bytes: Length
- Comment
- 8 Bytes: Date Added (FILETIME)
- 8 Bytes: Date Downloaded (FILETIME)
- 8 Bytes: Date Recorded Added (FILETIME)
- 8 Bytes: File Size
 
## Features ##

- Exports to CSV and HTML
- Extracts all record fields

## Download ##

- [v1.0.0](/downloads/FreeDownloadManagerForensics.v.1.0.0.zip)